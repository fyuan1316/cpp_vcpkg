find_package(GTest REQUIRED)

add_executable(multiply_test multiply_test.cpp)

target_link_libraries(multiply_test
  PRIVATE
  GTest::gtest GTest::gtest_main
  multiply
)

add_test(multiply_gtests multiply_test)

