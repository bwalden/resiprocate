set(INCLUDES
   ErrorCode.hxx
   TurnAsyncSocketHandler.hxx
   TurnAsyncSocket.hxx
   TurnAsyncTcpSocket.hxx
   TurnAsyncTlsSocket.hxx
   TurnAsyncUdpSocket.hxx
   TurnSocket.hxx
   TurnTcpSocket.hxx
   TurnTlsSocket.hxx
   TurnUdpSocket.hxx
   UdpEchoServer.hxx
)

add_library(reTurnClient
   TurnAsyncSocket.cxx
   TurnAsyncSocketHandler.cxx
   TurnAsyncTcpSocket.cxx
   TurnAsyncTlsSocket.cxx
   TurnAsyncUdpSocket.cxx
   TurnSocket.cxx
   TurnTcpSocket.cxx
   TurnTlsSocket.cxx
   TurnUdpSocket.cxx
   UdpEchoServer.cxx

   ${INCLUDES}
)

target_link_libraries(reTurnClient reTurnCommon)
set_target_properties(reTurnClient PROPERTIES FOLDER reTurn/client)
version_libname(reTurnClient)

install(TARGETS reTurnClient DESTINATION ${CMAKE_INSTALL_LIBDIR})
install_and_preserve_hierarchy(${CMAKE_INSTALL_INCLUDEDIR}/reTurn/client ${INCLUDES})

if(BUILD_TESTING)
    add_subdirectory(TurnLoadGenClient)
    add_subdirectory(test)
endif()
