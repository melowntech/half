# bump version here
set(half_VERSION 1.1)

define_module(LIBRARY half=${half_VERSION} DEPENDS)

set(half_SOURCES
  half.hpp
  dummy.cpp
)

add_library(half STATIC ${half_SOURCES})
set_target_properties(half PROPERTIES LINKER_LANGUAGE CXX)
buildsys_library(half)
