add_subdirectory(lib/googletest)

include_directories(${DIVISION_HEADERS_DIR})
include_directories(lib/googletest/googletest/include)

set(SOURCE_FILES main.cpp src/divider_tests.cpp)

add_executable(main_test ${SOURCE_FILES})
target_link_libraries(main_test target gtest)

# install(TARGETS divider_tests DESTINATION bin)

