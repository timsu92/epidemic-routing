build_lib_example(
  NAME epidemic-example
  SOURCE_FILES epidemic-example.cc
  LIBRARIES_TO_LINK
    ${libepidemic-routing}
    ${libwifi}
    ${libmesh}
    ${libapplications}
)

build_lib_example(
  NAME epidemic-benchmark
  SOURCE_FILES epidemic-benchmark.cc
  LIBRARIES_TO_LINK
    ${libepidemic-routing}
    ${libwifi}
    ${libmesh}
    ${libapplications}
)