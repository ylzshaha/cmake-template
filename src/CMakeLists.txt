add_subdirectory(target)
set(SOURCE_FILES main.cpp)

add_executable(main ${SOURCE_FILES})
target_link_libraries(main target)


#install(TARGETS divider DESTINATION ${DIVISIBLE_INSTALL_BIN_DIR})
