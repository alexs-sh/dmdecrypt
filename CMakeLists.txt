project("dmdecrypt" C)
cmake_minimum_required(VERSION 3.4)

find_package(OpenSSL REQUIRED SSL Crypto)

add_executable(${CMAKE_PROJECT_NAME} main.c)
target_include_directories(${CMAKE_PROJECT_NAME} PUBLIC "${OPENSSL_INCLUDE_DIR}")
target_link_libraries(${CMAKE_PROJECT_NAME} ${OPENSSL_LIBRARIES})
