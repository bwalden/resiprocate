set(INCLUDES
   AbandonServerTransaction.hxx
   AddTransport.hxx
   Aor.hxx
   ApiCheck.hxx
   ApiCheckList.hxx
   ApplicationMessage.hxx
   ApplicationSip.hxx
   Auth.hxx
   BasicDomainMatcher.hxx
   BasicNonceHelper.hxx
   BranchParameter.hxx
   CallId.hxx
   Cookie.hxx
   CancelableTimerQueue.hxx
   CancelClientInviteTransaction.hxx
   Compression.hxx
   ConnectionBase.hxx
   Connection.hxx
   ConnectionManager.hxx
   ConnectionTerminated.hxx
   ContentsFactoryBase.hxx
   ContentsFactory.hxx
   Contents.hxx
   CpimContents.hxx
   CSeqCategory.hxx
   DataParameter.hxx
   DateCategory.hxx
   DeprecatedDialog.hxx
   DialogInfoContents.hxx
   Dispatcher.hxx
   DnsInterface.hxx
   DnsResult.hxx
   DnsResultMessage.hxx
   DomainMatcher.hxx
   DtlsMessage.hxx
   DtmfPayloadContents.hxx
   Embedded.hxx
   EnableFlowTimer.hxx
   EventStackThread.hxx
   ExistsOrDataParameter.hxx
   ExistsParameter.hxx
   ExpiresCategory.hxx
   ExtendedDomainMatcher.hxx
   ExtensionHeader.hxx
   ExtensionParameter.hxx
   ExternalBodyContents.hxx
   FloatParameter.hxx
   GenericContents.hxx
   GenericPidfContents.hxx
   GenericUri.hxx
   HEPSipMessageLoggingHandler.hxx
   HeaderFieldValue.hxx
   HeaderFieldValueList.hxx
   HeaderHash.hxx
   Headers.hxx
   HeaderTypes.hxx
   Helper.hxx
   IntegerCategory.hxx
   IntegerParameter.hxx
   InternalTransport.hxx
   InteropHelper.hxx
   InterruptableStackThread.hxx
   InvalidContents.hxx
   InvokeAfterSocketCreationFunc.hxx
   KeepAliveMessage.hxx
   KeepAlivePong.hxx
   LazyParser.hxx
   MediaControlContents.hxx
   MarkListener.hxx
   MessageDecorator.hxx
   MessageFilterRule.hxx
   Message.hxx
   MessageWaitingContents.hxx
   MethodHash.hxx
   MethodTypes.hxx
   Mime.hxx
   MsgHeaderScanner.hxx
   MultipartAlternativeContents.hxx
   MultipartMixedContents.hxx
   MultipartRelatedContents.hxx
   MultipartSignedContents.hxx
   NameAddr.hxx
   NonceHelper.hxx
   OctetContents.hxx
   ParameterHash.hxx
   Parameter.hxx
   ParameterTypeEnums.hxx
   ParameterTypes.hxx
   ParserCategories.hxx
   ParserCategory.hxx
   ParserContainerBase.hxx
   ParserContainer.hxx
   Pidf.hxx
   Pkcs7Contents.hxx
   Pkcs8Contents.hxx
   PlainContents.hxx
   PollStatistics.hxx
   PrivacyCategory.hxx
   QuotedDataParameter.hxx
   QValue.hxx
   QValueParameter.hxx
   RAckCategory.hxx
   ReceivedParameter.hxx
   RemoveTransport.hxx
   RequestLine.hxx
   Rlmi.hxx
   RportParameter.hxx
   SdpContents.hxx
   SecurityAttributes.hxx
   SecurityTypes.hxx
   SendData.hxx
   SERNonceHelper.hxx
   ShutdownMessage.hxx
   SipConfigParse.hxx
   SipFrag.hxx
   SipMessage.hxx
   SipStack.hxx
   ssl/DtlsTransport.hxx
   ssl/MacSecurity.hxx
   ssl/Security.hxx
   ssl/TlsBaseTransport.hxx
   ssl/TlsConnection.hxx
   ssl/TlsTransport.hxx
   ssl/WinSecurity.hxx
   ssl/WssTransport.hxx
   ssl/WssConnection.hxx
   StackThread.hxx
   StartLine.hxx
   StatelessHandler.hxx
   StatisticsHandler.hxx
   StatisticsManager.hxx
   StatisticsMessage.hxx
   StatusLine.hxx
   StringCategory.hxx
   Symbols.hxx
   TcpBaseTransport.hxx
   TcpConnection.hxx
   TcpConnectState.hxx
   TcpTransport.hxx
   TerminateFlow.hxx
   TimeAccumulate.hxx
   TimerMessage.hxx
   TimerQueue.hxx
   Token.hxx
   TokenOrQuotedStringCategory.hxx
   TransactionController.hxx
   TransactionControllerThread.hxx
   TransactionMap.hxx
   TransactionMessage.hxx
   TransportSelectorThread.hxx
   TransactionState.hxx
   TransactionTerminated.hxx
   TransactionUser.hxx
   TransactionUserMessage.hxx
   TransportFailure.hxx
   Transport.hxx
   TransportSelector.hxx
   TransportThread.hxx
   TrickleIceContents.hxx
   TuIM.hxx
   Tuple.hxx
   TupleMarkManager.hxx
   TuSelector.hxx
   UdpTransport.hxx
   UInt32Category.hxx
   UInt32Parameter.hxx
   UnknownHeaderType.hxx
   UnknownParameter.hxx
   UnknownParameterType.hxx
   Uri.hxx
   ValueFifo.hxx
   Via.hxx
   WarningCategory.hxx
   Worker.hxx
   WorkerThread.hxx
   WsBaseTransport.hxx
   WsDecorator.hxx
   WsFrameExtractor.hxx
   WsTransport.hxx
   WsConnection.hxx
   WsConnectionBase.hxx
   WsConnectionValidator.hxx
   WsCookieContext.hxx
   WsCookieContextFactory.hxx
   X509Contents.hxx
   ZeroOutStatistics.hxx
)

add_library(resip
   Auth.cxx
   CSeqCategory.cxx
   CallId.cxx
   Cookie.cxx
   DateCategory.cxx
   gen/DayOfWeekHash.cxx
   DtmfPayloadContents.cxx
   ExpiresCategory.cxx
   GenericUri.cxx
   IntegerCategory.cxx
   InteropHelper.cxx
   UInt32Category.cxx
   Mime.cxx
   NameAddr.cxx
   ParserCategories.cxx
   RequestLine.cxx
   StatusLine.cxx
   StringCategory.cxx
   Token.cxx
   TokenOrQuotedStringCategory.cxx
   Via.cxx
   WarningCategory.cxx

   Aor.cxx
   ApiCheck.cxx
   ApplicationSip.cxx
   BasicDomainMatcher.cxx
   BasicNonceHelper.cxx
   BranchParameter.cxx
   Connection.cxx
   ConnectionBase.cxx
   ConnectionManager.cxx
   Contents.cxx
   ContentsFactoryBase.cxx
   CpimContents.cxx
   DataParameter.cxx
   DeprecatedDialog.cxx
   DialogInfoContents.cxx
   Dispatcher.cxx
   DnsInterface.cxx
   DnsResult.cxx
   DtlsMessage.cxx
   Embedded.cxx
   ExtensionParameter.cxx
   ExtensionHeader.cxx
   ExistsOrDataParameter.cxx
   ExistsParameter.cxx
   ExternalBodyContents.cxx
   ExtendedDomainMatcher.cxx
   QValue.cxx
   QValueParameter.cxx
   GenericContents.cxx
   GenericPidfContents.cxx
   HEPSipMessageLoggingHandler.cxx
   HeaderFieldValue.cxx
   HeaderFieldValueList.cxx
   gen/HeaderHash.cxx
   HeaderTypes.cxx
   Headers.cxx
   Helper.cxx
   IntegerParameter.cxx
   UInt32Parameter.cxx
   InternalTransport.cxx
   LazyParser.cxx
   MediaControlContents.cxx
   Message.cxx
   MessageWaitingContents.cxx
   gen/MethodHash.cxx
   MethodTypes.cxx
   gen/MonthHash.cxx
   MsgHeaderScanner.cxx
   MultipartAlternativeContents.cxx
   MultipartMixedContents.cxx
   MultipartRelatedContents.cxx
   MultipartSignedContents.cxx
   NonceHelper.cxx
   OctetContents.cxx
   Parameter.cxx
   gen/ParameterHash.cxx
   ParameterTypes.cxx
   ParserCategory.cxx
   ParserContainerBase.cxx
   Pidf.cxx
   Pkcs7Contents.cxx
   Pkcs8Contents.cxx
   PlainContents.cxx
   PrivacyCategory.cxx
   QuotedDataParameter.cxx
   RAckCategory.cxx
   ReceivedParameter.cxx
   Rlmi.cxx
   RportParameter.cxx
   SERNonceHelper.cxx
   SdpContents.cxx
   SecurityAttributes.cxx
   Compression.cxx
   SipConfigParse.cxx
   SipFrag.cxx
   SipMessage.cxx
   SipStack.cxx
   StackThread.cxx
   InterruptableStackThread.cxx
   EventStackThread.cxx
   StatisticsHandler.cxx
   StatisticsManager.cxx
   StatisticsMessage.cxx
   Symbols.cxx
   TcpBaseTransport.cxx
   TcpConnection.cxx
   TcpConnectState.cxx
   TcpTransport.cxx
   TimeAccumulate.cxx
   TimerMessage.cxx
   TimerQueue.cxx
   Tuple.cxx
   TupleMarkManager.cxx
   TransactionController.cxx
   MessageFilterRule.cxx
   TransactionUser.cxx
   TransactionUserMessage.cxx
   TransactionMap.cxx
   TransactionState.cxx
   Transport.cxx
   TransportThread.cxx
   TransportFailure.cxx
   TransportSelector.cxx
   TrickleIceContents.cxx
   TuIM.cxx
   TuSelector.cxx
   UdpTransport.cxx
   UnknownParameter.cxx
   Uri.cxx
   X509Contents.cxx
   KeepAliveMessage.cxx
   StatelessHandler.cxx
   InvalidContents.cxx
   WorkerThread.cxx
   WsBaseTransport.cxx
   WsFrameExtractor.cxx
   WsTransport.cxx
   WsConnection.cxx
   WsConnectionBase.cxx
   WsCookieContext.cxx
   WsDecorator.cxx

   ${INCLUDES}
)

target_add_conditional_sources(resip OPENSSL_FOUND
   ssl/DtlsTransport.cxx
   ssl/Security.cxx
   ssl/TlsBaseTransport.cxx
   ssl/TlsConnection.cxx
   ssl/TlsTransport.cxx
   ssl/WssConnection.cxx
   ssl/WssTransport.cxx
)

target_add_conditional_sources(resip APPLE
   ssl/MacSecurity.cxx
)

if(WIN32)
   target_add_conditional_sources(resip WITH_SSL
      ssl/WinSecurity.cxx
   )
endif()

set(GPERF_OPTS -C -D -E -L C++ -t --key-positions='*' --compare-strncmp)
# FIXME: we should put the generated files in ${PROJECT_BINARY_DIR}
#        and if we don't run gperf, we should copy the cached versions
#        to ${PROJECT_BINARY_DIR}
function(run_gperf)
   file(MAKE_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/gen)
   if(RUN_GPERF)
      add_custom_command(
         DEPENDS ${CMAKE_CURRENT_SOURCE_DIR}/${ARGV0}.gperf
         OUTPUT gen/${ARGV0}.cxx
         COMMAND gperf ${GPERF_OPTS} ${ARGV1} -Z ${ARGV0} ${CMAKE_CURRENT_SOURCE_DIR}/${ARGV0}.gperf > ${CMAKE_CURRENT_BINARY_DIR}/gen/${ARGV0}.cxx
      )
   else()
      file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/gen/${ARGV0}.cxx DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/gen)
   endif()
endfunction()

# With autotools, we would not run gperf automatically on every build.
# It is not always available on every platform.
# With CMake, we now take the inverse approach, it is run on every build
# but it can be disabled by changing RUN_GPERF to False
run_gperf(DayOfWeekHash)
run_gperf(HeaderHash --ignore-case)
run_gperf(MethodHash)
run_gperf(MonthHash)
run_gperf(ParameterHash --ignore-case)

target_add_conditional_sources(resip TRUE
   gen/DayOfWeekHash.cxx
   gen/HeaderHash.cxx
   gen/MethodHash.cxx
   gen/MonthHash.cxx
   gen/ParameterHash.cxx
)

if(WIN32)
   if(WITH_SSL)
      target_link_libraries(resip crypt32 Ncrypt)
   endif()
   # For whatever historical reason, on Windows the name of the library is not
   # resip but resiprocate.
   set_target_properties(resip PROPERTIES OUTPUT_NAME resiprocate)
elseif(APPLE)
   target_link_libraries(resip "-framework CoreFoundation")
   target_link_libraries(resip "-framework CoreServices")
   target_link_libraries(resip "-framework Security")
endif()

target_include_directories(resip PUBLIC $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}>)
target_link_libraries(resip ${opensigcomp_LIBRARIES} rutil)
version_libname(resip)
set_target_properties(resip PROPERTIES FOLDER resip)

install(TARGETS resip DESTINATION ${CMAKE_INSTALL_LIBDIR})
install_and_preserve_hierarchy(${CMAKE_INSTALL_INCLUDEDIR}/resip/stack ${INCLUDES})

if(BUILD_TESTING)
    add_subdirectory(test)
endif()
