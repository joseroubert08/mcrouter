SUBDIRS = lib . routes tools test

ACLOCAL_AMFLAGS = -I m4

noinst_LIBRARIES = libmcroutercore.a
bin_PROGRAMS = mcrouter

BUILT_SOURCES = \
  lib/network/McAsciiParser-gen.cpp

lib/network/McAsciiParser-gen.cpp: lib/network/McAsciiParser.rl
	ragel -G1 -o lib/network/McAsciiParser-gen.cpp lib/network/McAsciiParser.rl

CLEANFILES = \
  lib/network/McAsciiParser-gen.cpp

libmcroutercore_a_SOURCES = \
  AsyncLog.cpp \
  AsyncLog.h \
  AsyncTimer.h \
  AsyncWriter.cpp \
  AsyncWriter.h \
  AsyncWriterEntry.h \
  CallbackPool-inl.h \
  CallbackPool.h \
  CarbonRouterClient-inl.h \
  CarbonRouterClient.h \
  CarbonRouterClientBase.cpp \
  CarbonRouterClientBase.h \
  CarbonRouterInstance-inl.h \
  CarbonRouterInstance.cpp \
  CarbonRouterInstance.h \
  CarbonRouterInstanceBase.cpp \
  CarbonRouterInstanceBase.h \
  Clock.h \
  ConfigApi.cpp \
  ConfigApi.h \
  ConfigApiIf.h \
  ExponentialSmoothData.h \
  FileDataProvider.cpp \
  FileDataProvider.h \
  FileObserver.cpp \
  FileObserver.h \
  flavor.cpp \
  flavor.h \
  LeaseTokenMap.cpp \
  LeaseTokenMap.h \
  mcrouter_config-impl.h \
  mcrouter_config.cpp \
  mcrouter_config.h \
  mcrouter_options_list.h \
  McrouterClient.h \
  McrouterFiberContext.cpp \
  McrouterFiberContext.h \
  McrouterInstance.h \
  McrouterLogFailure.cpp \
  McrouterLogFailure.h \
  McrouterLogger.cpp \
  McrouterLogger.h \
  Observable-inl.h \
  Observable.h \
  options-template.h \
  options.cpp \
  options.h \
  OptionsUtil.cpp \
  OptionsUtil.h \
  PoolFactory.cpp \
  PoolFactory.h \
  Proxy-inl.h \
  Proxy.cpp \
  Proxy.h \
  ProxyBase-inl.h \
  ProxyBase.cpp \
  ProxyBase.h \
  ProxyConfig-inl.h \
  ProxyConfig.h \
  ProxyConfigBuilder.cpp \
  ProxyConfigBuilder.h \
  ProxyDestination-inl.h \
  ProxyDestination.cpp \
  ProxyDestination.h \
  ProxyDestinationMap.cpp \
  ProxyDestinationMap.h \
  ProxyRequestContext.cpp \
  ProxyRequestContext.h \
  ProxyRequestContextTyped-inl.h \
  ProxyRequestContextTyped.h \
  ProxyRequestLogger-inl.h \
  ProxyRequestLogger.cpp \
  ProxyRequestLogger.h \
  ProxyRequestPriority.h \
  ProxyStats.cpp \
  ProxyStats.h \
  ProxyThread-inl.h \
  ProxyThread.h \
  route.cpp \
  route.h \
  routes/AllAsyncRoute.cpp \
  routes/AllFastestRoute.cpp \
  routes/AllInitialRoute.cpp \
  routes/AllMajorityRoute.cpp \
  routes/AllSyncRoute.cpp \
  routes/AsynclogRoute.cpp \
  routes/AsynclogRoute.h \
  routes/BigValueRoute-inl.h \
  routes/BigValueRoute.cpp \
  routes/BigValueRoute.h \
  routes/BigValueRouteIf.h \
  routes/DefaultShadowPolicy.h \
  routes/DestinationRoute.h \
  routes/DevNullRoute.cpp \
  routes/DevNullRoute.h \
  routes/ErrorRoute.cpp \
  routes/ExtraRouteHandleProviderIf.h \
  routes/FailoverPolicy.h \
  routes/FailoverRateLimiter.cpp \
  routes/FailoverRateLimiter.h \
  routes/FailoverRoute-inl.h \
  routes/FailoverRoute.h \
  routes/FailoverWithExptimeRoute.cpp \
  routes/HashRoute.cpp \
  routes/HostIdRoute.cpp \
  routes/L1L2CacheRoute.cpp \
  routes/LatestRoute.h \
  routes/McExtraRouteHandleProvider-inl.h \
  routes/McExtraRouteHandleProvider.h \
  routes/McImportResolver.cpp \
  routes/McImportResolver.h \
  routes/McRouteHandleBuilder.h \
  routes/McRouteHandleProvider-inl.h \
  routes/McRouteHandleProvider.cpp \
  routes/McRouteHandleProvider.h \
  routes/McrouterRouteHandle.h \
  routes/MigrateRoute.cpp \
  routes/MissFailoverRoute.cpp \
  routes/MissFailoverRoute.h \
  routes/ModifyExptimeRoute.cpp \
  routes/ModifyExptimeRoute.h \
  routes/ModifyKeyRoute.cpp \
  routes/ModifyKeyRoute.h \
  routes/NullRoute.cpp \
  routes/OperationSelectorRoute-inl.h \
  routes/OperationSelectorRoute.h \
  routes/OutstandingLimitRoute.h \
  routes/PrefixSelectorRoute.h \
  routes/ProxyRoute-inl.h \
  routes/ProxyRoute.h \
  routes/RandomRoute.cpp \
  routes/RateLimiter.cpp \
  routes/RateLimiter.h \
  routes/RateLimitRoute.h \
  routes/RootRoute.h \
  routes/RouteHandleMap-inl.h \
  routes/RouteHandleMap.h \
  routes/RoutePolicyMap-inl.h \
  routes/RoutePolicyMap.h \
  routes/RouteSelectorMap.h \
  routes/ShadowRoute.h \
  routes/ShadowRoute-inl.h \
  routes/ShadowRouteIf.h \
  routes/ShardHashFunc.cpp \
  routes/ShardHashFunc.h \
  routes/ShardSplitRoute.cpp \
  routes/ShardSplitRoute.h \
  routes/ShardSplitter.cpp \
  routes/ShardSplitter.h \
  routes/SlowWarmupRoute.h \
  routes/SlowWarmUpRouteSettings.cpp \
  routes/SlowWarmupRouteSettings.h \
  routes/TimeProviderFunc.h \
  routes/WarmUpRoute.cpp \
  routes/WarmUpRoute.h \
  RoutingPrefix.cpp \
  RoutingPrefix.h \
  RuntimeVarsData.cpp \
  RuntimeVarsData.h \
  ServiceInfo-inl.h \
  ServiceInfo.h \
  stat_list.h \
  stats.cpp \
  stats.h \
  ThreadUtil.cpp \
  ThreadUtil.h \
  TkoCounters.h \
  TkoLog.cpp \
  TkoLog.h \
  TkoTracker.cpp \
  TkoTracker.h

mcrouter_SOURCES = \
  main.cpp \
  server.cpp \
  server.h \
  ServerOnRequest.h \
  standalone_options.h \
  standalone_options_list.h

libmcroutercore_a_CPPFLAGS = -I..

mcrouter_LDADD = libmcroutercore.a lib/libmcrouter.a
mcrouter_CPPFLAGS = -I..

clean-local:
	-rm -f lib/network/gen-cpp2/*.h \
	       lib/network/gen-cpp2/*.cpp \
	       lib/network/gen-cpp2/*.o \
	       lib/network/gen-cpp2/*.tcc

distclean-local:
	-rm -rf lib/network/gen-cpp2/
