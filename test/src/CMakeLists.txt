include_directories(../.. .)
add_definitions(-DHAVE_CONFIG_H)

set(SOURCE_FILES
        fswatch_test.c
        ../../libfswatch_config.h)

add_executable(fswatch_test ${SOURCE_FILES})
target_link_libraries(fswatch_test LINK_PUBLIC libfswatch)