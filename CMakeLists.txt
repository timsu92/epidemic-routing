build_lib(
  LIBNAME epidemic-routing  # can be later linked as ${libepidemic-routing}
  SOURCE_FILES  # equivalent to module.source
    model/epidemic-packet-queue.cc
    model/epidemic-packet.cc
    model/epidemic-tag.cc
    model/epidemic-routing-protocol.cc
    helper/epidemic-helper.cc
  HEADER_FILES # equivalent to headers.source
    model/epidemic-packet-queue.h
    model/epidemic-packet.h
    model/epidemic-tag.h
    model/epidemic-routing-protocol.h
    helper/epidemic-helper.h
  LIBRARIES_TO_LINK ${libinternet}
  TEST_SOURCES # equivalent to module_test.source
    test/epidemic-test-suite.cc
)