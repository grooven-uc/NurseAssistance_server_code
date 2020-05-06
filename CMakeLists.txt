cmake_minimum_required(VERSION 3.16)
project(NurseAssistance_server)

set(CMAKE_CXX_STANDARD 20)
SET(CMAKE_CXX_FLAGS -pthread)
add_executable(NurseAssistance_server main.cpp sockap/src/tcp_acceptor.cpp sockap/header/tcp_acceptor.h sockap/header/acceptor.h sockap/header/tcp_socket.h sockap/header/inet_address.h sockap/header/stream_socket.h sockap/header/socket.h sockap/header/sock_address.h sockap/header/platform.h sockap/version.h sockap/src/stream_socket.cpp sockap/src/exception.cpp sockap/header/exception.h sockap/src/acceptor.cpp sockap/src/inet_address.cpp sockap/src/socket.cpp ring_bell.cpp ring_bell.h)