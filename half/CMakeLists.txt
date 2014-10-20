define_module(LIBRARY half DEPENDS)

set(half_SOURCES
  half.hpp
  half.cpp
)

add_library(half STATIC ${half_SOURCES})
buildsys_library(half)
