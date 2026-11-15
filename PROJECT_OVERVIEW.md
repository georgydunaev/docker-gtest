# Project Overview: Ubuntu GoogleTest and Boost C++ Container Image (`docker-gtest`)

## Purpose and Scope

`docker-gtest` (`/botworkspace/docker-gtest`) provides a self-contained Ubuntu Docker build definition pre-configured with C++ build essentials, Boost libraries, `glog`, and a compiled installation of GoogleTest (`libgtest.a`) for running isolated C++ unit test suites.

## Repository Contents

- [Dockerfile](file:///botworkspace/docker-gtest/Dockerfile): Ubuntu container specification installing `build-essential`, `automake`, `libtool`, `flex`, `bison`, `pkg-config`, `g++`, `libssl-dev`, `libboost-all-dev` (`libboost-test-dev`, `libboost-program-options-dev`, `libboost-system-dev`, `libboost-filesystem-dev`), `libevent-dev`, and `libgoogle-glog-dev`, cloning `google/googletest`, and compiling `gtest-all.cc` into `/usr/lib/libgtest.a`.
- [README.md](file:///botworkspace/docker-gtest/README.md): Repository identifier.
