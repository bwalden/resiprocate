# escape=`

# Use the latest Windows Server Core image with .NET Framework 4.8.
FROM mcr.microsoft.com/dotnet/framework/sdk:4.8-windowsservercore-ltsc2019

# Install Chocolatey
RUN Set-ExecutionPolicy Bypass -Scope Process -Force; `
    $env:chocolateyUseWindowsCompression = 'true'; `
    [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; `
    iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

# Install Visual Studio 2019 Build Tools with VC Tools workload
RUN choco install visualstudio2019-workload-vctools -y

# Install Git
RUN choco install git -y

# Install Vcpkg
SHELL ["cmd", "/S", "/C"]
ENV VCPKG_DIR C:\vcpkg
RUN git clone https://github.com/microsoft/vcpkg.git %VCPKG_DIR% && `
    cd %VCPKG_DIR% && `
    .\bootstrap-vcpkg.bat && `
    vcpkg integrate install && `
    setx PATH "%PATH%;%VCPKG_DIR%"

# Install Vcpkg packages
RUN vcpkg install --triplet x64-windows asio berkeleydb boost cppunit openssl pcre

WORKDIR C:\jenkins
