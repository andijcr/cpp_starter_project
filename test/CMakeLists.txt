include(CTest)
CPMAddPackage("gh:doctest/doctest#2.4.7")

add_executable(tests tests.cpp)
target_link_libraries(tests PRIVATE project_warnings project_options doctest_with_main)
