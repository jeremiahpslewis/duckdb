add_library_unity(
  duckdb_operator_helper
  OBJECT
  physical_execute.cpp
  physical_explain_analyze.cpp
  physical_limit.cpp
  physical_limit_percent.cpp
  physical_load.cpp
  physical_pragma.cpp
  physical_prepare.cpp
  physical_reservoir_sample.cpp
  physical_set.cpp
  physical_streaming_sample.cpp
  physical_transaction.cpp
  physical_vacuum.cpp)
set(ALL_OBJECT_FILES
    ${ALL_OBJECT_FILES} $<TARGET_OBJECTS:duckdb_operator_helper>
    PARENT_SCOPE)
