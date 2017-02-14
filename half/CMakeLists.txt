# bump version here
set(half_VERSION 1.1)

define_module(LIBRARY half=${half_VERSION} DEPENDS)

set(half_SOURCES
  half.hpp
  half.cpp
)

add_library(half STATIC ${half_SOURCES})
buildsys_library(half)
