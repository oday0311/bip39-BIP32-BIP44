cmake_minimum_required(VERSION 3.10)
project(CL_BIP39_project)

INCLUDE_DIRECTORIES()
set(CMAKE_CXX_STANDARD 11)

SET(SOURCE_FILES                                  #设置变量，表示所有的源文件
        includeALL.h
        common.h
        bip32.h
        bignum256.cpp
        bip32.cpp
        bip39.cpp
        ecdsa.cpp
        endian.cpp
        hash.cpp
        hmac_drbg.cpp
        Hmacsha512.cpp
        main.cpp
        masterpublicKey.cpp
        parseTransaction.cpp
        pbkdf2.cpp
        sha256.cpp
        Transaction.cpp
        )


add_executable(CL_BIP39_project ${SOURCE_FILES})
