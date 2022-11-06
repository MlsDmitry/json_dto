cmake_minimum_required(VERSION 3.9)

project(json_dto VERSION 0.3.1 LANGUAGES CXX)


set(CMAKE_CXX_STANDARD          14 )
set(CMAKE_CXX_STANDARD_REQUIRED ON )

set(JSON_DTO_HEADERS include/json_dto/pub.hpp)

add_library(json-dto INTERFACE)
add_library(json-dto::json-dto ALIAS json-dto)


target_include_directories(json-dto INTERFACE include)
