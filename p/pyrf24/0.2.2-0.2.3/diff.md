# Comparing `tmp/pyrf24-0.2.2.tar.gz` & `tmp/pyrf24-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrf24-0.2.2.tar", last modified: Thu Jan 19 11:39:58 2023, max compression
+gzip compressed data, was "pyrf24-0.2.3.tar", last modified: Fri Jul 28 01:25:12 2023, max compression
```

## Comparing `pyrf24-0.2.2.tar` & `pyrf24-0.2.3.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.620757 pyrf24-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-01-19 10:28:41.000000 pyrf24-0.2.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-01-19 10:28:41.000000 pyrf24-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-01-19 10:28:41.000000 pyrf24-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-01-19 11:39:58.620757 pyrf24-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-01-19 10:28:41.000000 pyrf24-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.596757 pyrf24-0.2.2/RF24/
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    67839 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/RF24.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    96251 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/RF24.h
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/RF24_config.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.596757 pyrf24-0.2.2/RF24/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/AutoConfig_RF24_DRIVER.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/CPackInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/Cache.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/CompilerWarnings.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/GetLibInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/Sanitizers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/StandardProjectSettings.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/StaticAnalyzers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/detectCPU.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/cmake/pico_sdk_import.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/nRF24L01.h
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/printf.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.596757 pyrf24-0.2.2/RF24/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.596757 pyrf24-0.2.2/RF24/utility/LittleWire/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/LittleWire/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/LittleWire/includes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.596757 pyrf24-0.2.2/RF24/utility/MRAA/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/gpio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/gpio.h
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/includes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/MRAA/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.600757 pyrf24-0.2.2/RF24/utility/RPi/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    61079 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/bcm2835.c
--rw-r--r--   0 runner    (1001) docker     (123)    96902 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/bcm2835.h
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/includes.h
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/interrupt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/interrupt.h
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/RPi/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.600757 pyrf24-0.2.2/RF24/utility/SPIDEV/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/gpio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/gpio.h
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/includes.h
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/interrupt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/interrupt.h
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/SPIDEV/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.600757 pyrf24-0.2.2/RF24/utility/pigpio/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/compatibility.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/compatibility.h
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/gpio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/gpio.h
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/includes.h
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/interrupt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/interrupt.h
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/pigpio/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.600757 pyrf24-0.2.2/RF24/utility/wiringPi/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/wiringPi/RF24_arch_config.h
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/wiringPi/includes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/wiringPi/spi.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24/utility/wiringPi/spi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.600757 pyrf24-0.2.2/RF24Mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18005 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/RF24Mesh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/RF24Mesh.h
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/RF24Mesh_config.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.600757 pyrf24-0.2.2/RF24Mesh/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/CPackInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/Cache.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/CompilerWarnings.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/GetLibInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/StandardProjectSettings.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/detectCPU.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/enableNcursesExample.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Mesh/cmake/usePicoSDK.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.604757 pyrf24-0.2.2/RF24Network/
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46083 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/RF24Network.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    41487 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/RF24Network.h
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/RF24Network_config.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.604757 pyrf24-0.2.2/RF24Network/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/CPackInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/Cache.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/CompilerWarnings.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/GetLibInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/StandardProjectSettings.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/detectCPU.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-19 10:28:45.000000 pyrf24-0.2.2/RF24Network/cmake/usePicoSDK.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.604757 pyrf24-0.2.2/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-01-19 10:28:41.000000 pyrf24-0.2.2/cmake/using_flags.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.604757 pyrf24-0.2.2/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/.codespell-ignore-lines
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.592756 pyrf24-0.2.2/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.612757 pyrf24-0.2.2/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.612757 pyrf24-0.2.2/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.612757 pyrf24-0.2.2/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.616757 pyrf24-0.2.2/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.616757 pyrf24-0.2.2/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.616757 pyrf24-0.2.2/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-19 10:28:45.000000 pyrf24-0.2.2/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-01-19 10:28:41.000000 pyrf24-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.616757 pyrf24-0.2.2/pyrf24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-01-19 11:39:58.000000 pyrf24-0.2.2/pyrf24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-01-19 11:39:58.000000 pyrf24-0.2.2/pyrf24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 11:39:58.000000 pyrf24-0.2.2/pyrf24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 11:39:58.000000 pyrf24-0.2.2/pyrf24.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-19 11:39:58.000000 pyrf24-0.2.2/pyrf24.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-19 10:28:41.000000 pyrf24-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-19 10:28:41.000000 pyrf24-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 11:39:58.620757 pyrf24-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-01-19 10:28:41.000000 pyrf24-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.620757 pyrf24-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)    59810 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyRF24.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyRF24Mesh.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23537 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyRF24Network.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:39:58.620757 pyrf24-0.2.2/src/pyrf24/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyrf24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35160 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyrf24/fake_ble.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyrf24/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyrf24/rf24.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyrf24/rf24_mesh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-01-19 10:28:41.000000 pyrf24-0.2.2/src/pyrf24/rf24_network.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.078369 pyrf24-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-28 00:09:04.000000 pyrf24-0.2.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-28 00:09:04.000000 pyrf24-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-28 00:09:04.000000 pyrf24-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-28 01:25:12.078369 pyrf24-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-07-28 00:09:04.000000 pyrf24-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.062368 pyrf24-0.2.3/RF24/
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    68018 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/RF24.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    96322 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/RF24.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/RF24_config.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.062368 pyrf24-0.2.3/RF24/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/AutoConfig_RF24_DRIVER.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/CPackInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/Cache.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/CompilerWarnings.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/GetLibInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/Sanitizers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/StaticAnalyzers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/detectCPU.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/cmake/pico_sdk_import.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/nRF24L01.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/printf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.062368 pyrf24-0.2.3/RF24/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.062368 pyrf24-0.2.3/RF24/utility/LittleWire/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/LittleWire/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/LittleWire/includes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.062368 pyrf24-0.2.3/RF24/utility/MRAA/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/gpio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/includes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/MRAA/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.066369 pyrf24-0.2.3/RF24/utility/RPi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61079 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/bcm2835.c
+-rw-r--r--   0 runner    (1001) docker     (123)    96902 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/bcm2835.h
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/includes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/interrupt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/RPi/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.066369 pyrf24-0.2.3/RF24/utility/SPIDEV/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/gpio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/includes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/interrupt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/SPIDEV/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.066369 pyrf24-0.2.3/RF24/utility/pigpio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/compatibility.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/compatibility.h
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/gpio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/gpio.h
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/includes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/interrupt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/interrupt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/pigpio/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.066369 pyrf24-0.2.3/RF24/utility/wiringPi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/wiringPi/RF24_arch_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/wiringPi/includes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/wiringPi/spi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24/utility/wiringPi/spi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.066369 pyrf24-0.2.3/RF24Mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19586 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/RF24Mesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/RF24Mesh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/RF24Mesh_config.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.070369 pyrf24-0.2.3/RF24Mesh/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/CPackInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/Cache.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/CompilerWarnings.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/GetLibInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/detectCPU.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/enableNcursesExample.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Mesh/cmake/usePicoSDK.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.070369 pyrf24-0.2.3/RF24Network/
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/RF24Network.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    42775 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/RF24Network.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/RF24Network_config.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.070369 pyrf24-0.2.3/RF24Network/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/CPackInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/Cache.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/CompilerWarnings.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/GetLibInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/detectCPU.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-28 00:09:10.000000 pyrf24-0.2.3/RF24Network/cmake/usePicoSDK.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.070369 pyrf24-0.2.3/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-28 00:09:04.000000 pyrf24-0.2.3/cmake/using_flags.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.070369 pyrf24-0.2.3/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.058368 pyrf24-0.2.3/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.074369 pyrf24-0.2.3/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.074369 pyrf24-0.2.3/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28518 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52930 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.074369 pyrf24-0.2.3/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    31450 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79416 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.074369 pyrf24-0.2.3/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.074369 pyrf24-0.2.3/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.078369 pyrf24-0.2.3/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-28 00:09:10.000000 pyrf24-0.2.3/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-28 00:09:04.000000 pyrf24-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.078369 pyrf24-0.2.3/pyrf24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-28 01:25:11.000000 pyrf24-0.2.3/pyrf24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-28 01:25:12.000000 pyrf24-0.2.3/pyrf24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:25:11.000000 pyrf24-0.2.3/pyrf24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:25:11.000000 pyrf24-0.2.3/pyrf24.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 01:25:11.000000 pyrf24-0.2.3/pyrf24.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 00:09:04.000000 pyrf24-0.2.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 00:09:04.000000 pyrf24-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:25:12.078369 pyrf24-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-28 00:09:04.000000 pyrf24-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.078369 pyrf24-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    59810 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyRF24.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyRF24Mesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23537 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyRF24Network.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:25:12.078369 pyrf24-0.2.3/src/pyrf24/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyrf24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35160 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyrf24/fake_ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyrf24/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyrf24/rf24.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyrf24/rf24_mesh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-28 00:09:04.000000 pyrf24-0.2.3/src/pyrf24/rf24_network.pyi
```

### Comparing `pyrf24-0.2.2/CMakeLists.txt` & `pyrf24-0.2.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/LICENSE` & `pyrf24-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/MANIFEST.in` & `pyrf24-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/PKG-INFO` & `pyrf24-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrf24
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package for the wrapping nRF24 related C++ libraries.
 Author-email: Brendan Doherty <2bndy5@gmail.com>
 License: GPLv2
 Project-URL: Documentation, http://nRF24.github.io/pyRF24
 Project-URL: Source, https://github.com/nRF24/pyRF24
 Project-URL: Tracker, https://github.com/nRF24/pyRF24/issues
 Keywords: nrf24l01,nRF24L01+,raspberry,pi,driver,radio,transceiver
```

### Comparing `pyrf24-0.2.2/README.rst` & `pyrf24-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/CMakeLists.txt` & `pyrf24-0.2.3/RF24/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/LICENSE` & `pyrf24-0.2.3/RF24/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/RF24.cpp` & `pyrf24-0.2.3/RF24/RF24.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,22 @@
 #endif // !defined(RF24_LINUX)
 }
 
 /****************************************************************************/
 
 void RF24::ce(bool level)
 {
+#ifndef RF24_LINUX
     //Allow for 3-pin use on ATTiny
     if (ce_pin != csn_pin) {
+#endif
         digitalWrite(ce_pin, level);
+#ifndef RF24_LINUX
     }
+#endif
 }
 
 /****************************************************************************/
 
 inline void RF24::beginTransaction()
 {
 #if defined(RF24_SPI_TRANSACTIONS)
@@ -569,24 +573,24 @@
     delete[] read_buffer;
     return offset;
 }
 #endif // !defined(MINIMAL)
 
 /****************************************************************************/
 
-RF24::RF24(uint16_t _cepin, uint16_t _cspin, uint32_t _spi_speed)
+RF24::RF24(rf24_gpio_pin_t _cepin, rf24_gpio_pin_t _cspin, uint32_t _spi_speed)
     : ce_pin(_cepin), csn_pin(_cspin), spi_speed(_spi_speed), payload_size(32), _is_p_variant(false), _is_p0_rx(false), addr_width(5), dynamic_payloads_enabled(true), csDelay(5)
 {
     _init_obj();
 }
 
 /****************************************************************************/
 
 RF24::RF24(uint32_t _spi_speed)
-    : ce_pin(0xFFFF), csn_pin(0xFFFF), spi_speed(_spi_speed), payload_size(32), _is_p_variant(false), _is_p0_rx(false), addr_width(5), dynamic_payloads_enabled(true), csDelay(5)
+    : ce_pin(RF24_PIN_INVALID), csn_pin(RF24_PIN_INVALID), spi_speed(_spi_speed), payload_size(32), _is_p_variant(false), _is_p0_rx(false), addr_width(5), dynamic_payloads_enabled(true), csDelay(5)
 {
     _init_obj();
 }
 
 /****************************************************************************/
 
 void RF24::_init_obj()
@@ -952,26 +956,26 @@
 {
     _spi = spiBus;
     return _init_pins() && _init_radio();
 }
 
 /****************************************************************************/
 
-bool RF24::begin(_SPI* spiBus, uint16_t _cepin, uint16_t _cspin)
+bool RF24::begin(_SPI* spiBus, rf24_gpio_pin_t _cepin, rf24_gpio_pin_t _cspin)
 {
     ce_pin = _cepin;
     csn_pin = _cspin;
     return begin(spiBus);
 }
 
 #endif // defined (RF24_SPI_PTR) || defined (DOXYGEN_FORCED)
 
 /****************************************************************************/
 
-bool RF24::begin(uint16_t _cepin, uint16_t _cspin)
+bool RF24::begin(rf24_gpio_pin_t _cepin, rf24_gpio_pin_t _cspin)
 {
     ce_pin = _cepin;
     csn_pin = _cspin;
     return begin();
 }
 
 /****************************************************************************/
@@ -995,14 +999,15 @@
 
     _SPI.begin(csn_pin, spi_speed);
 
 #elif defined(XMEGA_D3)
     _spi->begin(csn_pin);
 
 #elif defined(RF24_RP2)
+    _spi = new SPI();
     _spi->begin(PICO_DEFAULT_SPI ? spi1 : spi0);
 
 #else // using an Arduino platform || defined (LITTLEWIRE)
 
     #if defined(RF24_SPI_PTR)
     _spi->begin();
     #else  // !defined(RF24_SPI_PTR)
@@ -1142,15 +1147,15 @@
     return read_register(SETUP_AW) == (addr_width - static_cast<uint8_t>(2));
 }
 
 /****************************************************************************/
 
 bool RF24::isValid()
 {
-    return ce_pin != 0xFFFF && csn_pin != 0xFFFF;
+    return ce_pin != RF24_PIN_INVALID && csn_pin != RF24_PIN_INVALID;
 }
 
 /****************************************************************************/
 
 void RF24::startListening(void)
 {
 #if !defined(RF24_TINY) && !defined(LITTLEWIRE)
@@ -1512,15 +1517,16 @@
     return result;
 }
 
 /****************************************************************************/
 
 bool RF24::available(void)
 {
-    return available(NULL);
+    uint8_t pipe = 0;
+    return available(&pipe);
 }
 
 /****************************************************************************/
 
 bool RF24::available(uint8_t* pipe_num)
 {
     // get implied RX FIFO empty flag from status byte
```

### Comparing `pyrf24-0.2.2/RF24/RF24.h` & `pyrf24-0.2.3/RF24/RF24.h`

 * *Files 1% similar despite different names*

```diff
@@ -117,27 +117,27 @@
 private:
 #ifdef SOFTSPI
     SoftSPI<SOFT_SPI_MISO_PIN, SOFT_SPI_MOSI_PIN, SOFT_SPI_SCK_PIN, SPI_MODE> spi;
 #elif defined(SPI_UART)
     SPIUARTClass uspi;
 #endif
 
-#if defined(RF24_LINUX) || defined(XMEGA_D3) || defined(RF24_RP2) /* XMEGA can use SPI class */
+#if defined(RF24_LINUX) || defined(XMEGA_D3) /* XMEGA can use SPI class */
     SPI spi;
 #endif // defined (RF24_LINUX) || defined (XMEGA_D3)
 #if defined(RF24_SPI_PTR)
     _SPI* _spi;
 #endif // defined (RF24_SPI_PTR)
 #if defined(MRAA)
     GPIO gpio;
 #endif
 
-    uint16_t ce_pin;    /* "Chip Enable" pin, activates the RX or TX role */
-    uint16_t csn_pin;   /* SPI Chip select */
-    uint32_t spi_speed; /* SPI Bus Speed */
+    rf24_gpio_pin_t ce_pin;  /* "Chip Enable" pin, activates the RX or TX role */
+    rf24_gpio_pin_t csn_pin; /* SPI Chip select */
+    uint32_t spi_speed;      /* SPI Bus Speed */
 #if defined(RF24_LINUX) || defined(XMEGA_D3) || defined(RF24_RP2)
     uint8_t spi_rxbuff[32 + 1]; //SPI receive buffer (payload max 32 bytes)
     uint8_t spi_txbuff[32 + 1]; //SPI transmit buffer (payload max 32 bytes + 1 byte for the command)
 #endif
     uint8_t status;                   /* The status byte returned from every SPI transaction */
     uint8_t payload_size;             /* Fixed size of payloads */
     uint8_t pipe0_reading_address[5]; /* Last address set on pipe 0 for reading. */
@@ -197,27 +197,28 @@
      * and send in the unique pins that this chip is connected to.
      *
      * See [Related Pages](pages.html) for device specific information
      *
      * @param _cepin The pin attached to Chip Enable on the RF module
      * @param _cspin The pin attached to Chip Select (often labeled CSN) on the radio module.
      * - For the Arduino Due board, the [Arduino Due extended SPI feature](https://www.arduino.cc/en/Reference/DueExtendedSPI)
-     * is not supported. This means that the Due's pins 4, 10, or 52 are not mandated options (can use any digital output pin) for the radio's CSN pin.
+     * is not supported. This means that the Due's pins 4, 10, or 52 are not mandated options (can use any digital output pin) for
+     * the radio's CSN pin.
      * @param _spi_speed The SPI speed in Hz ie: 1000000 == 1Mhz
      * - Users can specify default SPI speed by modifying @ref RF24_SPI_SPEED in @ref RF24_config.h
      *     - For Arduino, the default SPI speed will only be properly configured this way on devices supporting SPI TRANSACTIONS
      *     - Older/Unsupported Arduino devices will use a default clock divider & settings configuration
      *     - For Linux: The old way of setting SPI speeds using BCM2835 driver enums has been removed as of v1.3.7
      */
-    RF24(uint16_t _cepin, uint16_t _cspin, uint32_t _spi_speed = RF24_SPI_SPEED);
+    RF24(rf24_gpio_pin_t _cepin, rf24_gpio_pin_t _cspin, uint32_t _spi_speed = RF24_SPI_SPEED);
 
     /**
      * A constructor for initializing the radio's hardware dynamically
-     * @warning You MUST use begin(uint16_t, uint16_t) or begin(_SPI*, uint16_t, uint16_t) to pass both the digital output pin
-     * numbers connected to the radio's CE and CSN pins.
+     * @warning You MUST use begin(rf24_gpio_pin_t, rf24_gpio_pin_t) or begin(_SPI*, rf24_gpio_pin_t, rf24_gpio_pin_t) to pass both the
+     * digital output pin numbers connected to the radio's CE and CSN pins.
      * @param _spi_speed The SPI speed in Hz ie: 1000000 == 1Mhz
      * - Users can specify default SPI speed by modifying @ref RF24_SPI_SPEED in @ref RF24_config.h
      *     - For Arduino, the default SPI speed will only be properly configured this way on devices supporting SPI TRANSACTIONS
      *     - Older/Unsupported Arduino devices will use a default clock divider & settings configuration
      *     - For Linux: The old way of setting SPI speeds using BCM2835 driver enums has been removed as of v1.3.7
      */
     RF24(uint32_t _spi_speed = RF24_SPI_SPEED);
@@ -277,27 +278,27 @@
      * - For the Arduino Due board, the [Arduino Due extended SPI feature](https://www.arduino.cc/en/Reference/DueExtendedSPI)
      * is not supported. This means that the Due's pins 4, 10, or 52 are not mandated options (can use any digital output pin) for the radio's CSN pin.
      *
      * @see Review the [Arduino support page](md_docs_arduino.html).
      *
      * @return same result as begin()
      */
-    bool begin(_SPI* spiBus, uint16_t _cepin, uint16_t _cspin);
+    bool begin(_SPI* spiBus, rf24_gpio_pin_t _cepin, rf24_gpio_pin_t _cspin);
 #endif // defined (RF24_SPI_PTR) || defined (DOXYGEN_FORCED)
 
     /**
      * Same as begin(), but allows dynamically specifying a CE pin
      * and CSN pin to use.
      * @param _cepin The pin attached to Chip Enable on the RF module
      * @param _cspin The pin attached to Chip Select (often labeled CSN) on the radio module.
      * - For the Arduino Due board, the [Arduino Due extended SPI feature](https://www.arduino.cc/en/Reference/DueExtendedSPI)
      * is not supported. This means that the Due's pins 4, 10, or 52 are not mandated options (can use any digital output pin) for the radio's CSN pin.
      * @return same result as begin()
      */
-    bool begin(uint16_t _cepin, uint16_t _cspin);
+    bool begin(rf24_gpio_pin_t _cepin, rf24_gpio_pin_t _cspin);
 
     /**
      * Checks if the chip is connected to the SPI bus
      */
     bool isChipConnected();
 
     /**
```

### Comparing `pyrf24-0.2.2/RF24/RF24_config.h` & `pyrf24-0.2.3/RF24/RF24_config.h`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,27 @@
 
 #elif defined(TEENSYDUINO) //Teensy
     #include "utility/Teensy/RF24_arch_config.h"
 
 #else //Everything else
     #include <Arduino.h>
 
+    #ifdef NUM_DIGITAL_PINS
+        #if NUM_DIGITAL_PINS < 255
+typedef uint8_t rf24_gpio_pin_t;
+            #define RF24_PIN_INVALID 0xFF
+        #else
+typedef uint16_t rf24_gpio_pin_t;
+            #define RF24_PIN_INVALID 0xFFFF
+        #endif
+    #else
+typedef uint16_t rf24_gpio_pin_t;
+        #define RF24_PIN_INVALID 0xFFFF
+    #endif
+
     #if defined(ARDUINO) && !defined(__arm__) && !defined(__ARDUINO_X86__)
         #if defined SPI_UART
             #include <SPI_UART.h>
             #define _SPI uspi
         #elif defined(SOFTSPI)
             // change these pins to your liking
             //
```

### Comparing `pyrf24-0.2.2/RF24/cmake/AutoConfig_RF24_DRIVER.cmake` & `pyrf24-0.2.3/RF24/cmake/AutoConfig_RF24_DRIVER.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/CPackInfo.cmake` & `pyrf24-0.2.3/RF24/cmake/CPackInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/Cache.cmake` & `pyrf24-0.2.3/RF24/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/CompilerWarnings.cmake` & `pyrf24-0.2.3/RF24/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/GetLibInfo.cmake` & `pyrf24-0.2.3/RF24/cmake/GetLibInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/PreventInSourceBuilds.cmake` & `pyrf24-0.2.3/RF24/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/Sanitizers.cmake` & `pyrf24-0.2.3/RF24/cmake/Sanitizers.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/StandardProjectSettings.cmake` & `pyrf24-0.2.3/RF24/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/StaticAnalyzers.cmake` & `pyrf24-0.2.3/RF24/cmake/StaticAnalyzers.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/detectCPU.cmake` & `pyrf24-0.2.3/RF24/cmake/detectCPU.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/cmake/pico_sdk_import.cmake` & `pyrf24-0.2.3/RF24/cmake/pico_sdk_import.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/nRF24L01.h` & `pyrf24-0.2.3/RF24/nRF24L01.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/printf.h` & `pyrf24-0.2.3/RF24/printf.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/CMakeLists.txt` & `pyrf24-0.2.3/RF24/utility/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/LittleWire/RF24_arch_config.h` & `pyrf24-0.2.3/RF24/utility/LittleWire/RF24_arch_config.h`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 // GCC a Arduino Missing
 #define _BV(x)           (1 << (x))
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define pgm_read_byte(p) (*(const unsigned char*)(p))
 #define pgm_read_ptr(p)  (*(void* const*)(p))
 
 //typedef uint16_t prog_uint16_t;
+typedef uint8_t rf24_gpio_pin_t;
+#define RF24_PIN_INVALID 0xFF
+
 #define PSTR(x)  (x)
 #define printf_P printf
 #define strlen_P strlen
 #define PROGMEM
 #define PRIPSTR "%s"
 
 #ifdef SERIAL_DEBUG
```

### Comparing `pyrf24-0.2.2/RF24/utility/MRAA/RF24_arch_config.h` & `pyrf24-0.2.3/RF24/utility/MRAA/RF24_arch_config.h`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define pgm_read_byte(p) (*(const unsigned char*)(p))
 #define pgm_read_ptr(p)  (*(void* const*)(p))
 #define _SPI             spi
 
 #define RF24_LINUX
 //typedef uint16_t prog_uint16_t;
+typedef uint16_t rf24_gpio_pin_t;
+#define RF24_PIN_INVALID 0xFFFF
+
 #define PSTR(x)   (x)
 #define printf_P  printf
 #define sprintf_P sprintf
 #define strlen_P  strlen
 #define PROGMEM
 #define PRIPSTR "%s"
```

### Comparing `pyrf24-0.2.2/RF24/utility/MRAA/compatibility.cpp` & `pyrf24-0.2.3/RF24/utility/MRAA/compatibility.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/MRAA/gpio.cpp` & `pyrf24-0.2.3/RF24/utility/MRAA/gpio.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/MRAA/gpio.h` & `pyrf24-0.2.3/RF24/utility/MRAA/gpio.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/MRAA/spi.cpp` & `pyrf24-0.2.3/RF24/utility/MRAA/spi.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/MRAA/spi.h` & `pyrf24-0.2.3/RF24/utility/MRAA/spi.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/RPi/RF24_arch_config.h` & `pyrf24-0.2.3/RF24/utility/RPi/RF24_arch_config.h`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 // GCC a Arduino Missing
 #define _BV(x)           (1 << (x))
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define pgm_read_byte(p) (*(const unsigned char*)(p))
 #define pgm_read_ptr(p)  (*(void* const*)(p))
 
 //typedef uint16_t prog_uint16_t;
+typedef uint8_t rf24_gpio_pin_t;
+#define RF24_PIN_INVALID 0xFF
+
 #define PSTR(x)  (x)
 #define printf_P printf
 #define strlen_P strlen
 #define PROGMEM
 #define PRIPSTR "%s"
 
 #ifdef SERIAL_DEBUG
```

### Comparing `pyrf24-0.2.2/RF24/utility/RPi/bcm2835.c` & `pyrf24-0.2.3/RF24/utility/RPi/bcm2835.c`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/RPi/bcm2835.h` & `pyrf24-0.2.3/RF24/utility/RPi/bcm2835.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/RPi/interrupt.h` & `pyrf24-0.2.3/RF24/utility/RPi/interrupt.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/RPi/spi.cpp` & `pyrf24-0.2.3/RF24/utility/RPi/spi.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/RPi/spi.h` & `pyrf24-0.2.3/RF24/utility/RPi/spi.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/RF24_arch_config.h` & `pyrf24-0.2.3/RF24/utility/SPIDEV/RF24_arch_config.h`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,17 @@
         #define PROGMEM __attribute__((section(".progmem.data")))
         #undef PSTR
         #define PSTR(s) (__extension__({static const char __c[] PROGMEM = (s); &__c[0]; }))
     #endif
 #endif
 
 typedef uint16_t prog_uint16_t;
+typedef uint16_t rf24_gpio_pin_t;
+#define RF24_PIN_INVALID 0xFFFF
+
 #define PSTR(x)  (x)
 #define printf_P printf
 #define strlen_P strlen
 #define PROGMEM
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define PRIPSTR          "%s"
 #define pgm_read_byte(p) (*(const unsigned char*)(p))
```

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/compatibility.cpp` & `pyrf24-0.2.3/RF24/utility/SPIDEV/compatibility.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/compatibility.h` & `pyrf24-0.2.3/RF24/utility/SPIDEV/compatibility.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/gpio.cpp` & `pyrf24-0.2.3/RF24/utility/SPIDEV/gpio.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/gpio.h` & `pyrf24-0.2.3/RF24/utility/SPIDEV/gpio.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/interrupt.h` & `pyrf24-0.2.3/RF24/utility/SPIDEV/interrupt.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/spi.cpp` & `pyrf24-0.2.3/RF24/utility/SPIDEV/spi.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/SPIDEV/spi.h` & `pyrf24-0.2.3/RF24/utility/SPIDEV/spi.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/pigpio/RF24_arch_config.h` & `pyrf24-0.2.3/RF24/utility/pigpio/RF24_arch_config.h`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 
 #if RF24_SPI_SPEED > 1000000
     #undef RF24_SPI_SPEED
     #define RF24_SPI_SPEED 1000000
 #endif
 
 typedef uint16_t prog_uint16_t;
+typedef uint8_t rf24_gpio_pin_t;
+#define RF24_PIN_INVALID 0xFF
+
 #define PSTR(x)  (x)
 #define printf_P printf
 #define strlen_P strlen
 #define PROGMEM
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define PRIPSTR          "%s"
 #define pgm_read_byte(p) (*(const unsigned char*)(p))
```

### Comparing `pyrf24-0.2.2/RF24/utility/pigpio/compatibility.cpp` & `pyrf24-0.2.3/RF24/utility/pigpio/compatibility.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/pigpio/compatibility.h` & `pyrf24-0.2.3/RF24/utility/pigpio/compatibility.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/pigpio/gpio.h` & `pyrf24-0.2.3/RF24/utility/pigpio/gpio.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/pigpio/interrupt.h` & `pyrf24-0.2.3/RF24/utility/pigpio/interrupt.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/pigpio/spi.cpp` & `pyrf24-0.2.3/RF24/utility/pigpio/spi.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 void SPI::begin(int busNo, uint32_t spi_speed)
 {
     if (this->spiIsInitialized) {
         return;
     }
     spiIsInitialized = true;
     gpioInitialise();
-    spiHandle = spiOpen(busNo, spi_speed, 0);
+    spiHandle = spiOpen((unsigned int)(busNo & 2), spi_speed, (unsigned int)((busNo / 10) << 7));
 }
 
 void SPI::init(uint32_t speed)
 {
 }
 
 uint8_t SPI::transfer(char tx)
```

### Comparing `pyrf24-0.2.2/RF24/utility/pigpio/spi.h` & `pyrf24-0.2.3/RF24/utility/pigpio/spi.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/wiringPi/RF24_arch_config.h` & `pyrf24-0.2.3/RF24/utility/wiringPi/RF24_arch_config.h`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     #undef PROGMEM
     #define PROGMEM __attribute__((section(".progmem.data")))
     #undef PSTR
     #define PSTR(s) (__extension__({static const char __c[] PROGMEM = (s); &__c[0]; }))
 #endif
 
 typedef uint16_t prog_uint16_t;
+typedef uint8_t rf24_gpio_pin_t;
+#define RF24_PIN_INVALID 0xFF
+
 #define PSTR(x)  (x)
 #define printf_P printf
 #define strlen_P strlen
 #define PROGMEM
 #define pgm_read_word(p) (*(const unsigned short*)(p))
 #define PRIPSTR          "%s"
 #define pgm_read_byte(p) (*(const unsigned char*)(p))
```

### Comparing `pyrf24-0.2.2/RF24/utility/wiringPi/spi.cpp` & `pyrf24-0.2.3/RF24/utility/wiringPi/spi.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24/utility/wiringPi/spi.h` & `pyrf24-0.2.3/RF24/utility/wiringPi/spi.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/CMakeLists.txt` & `pyrf24-0.2.3/RF24Mesh/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/LICENSE` & `pyrf24-0.2.3/RF24Mesh/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/RF24Mesh.cpp` & `pyrf24-0.2.3/RF24Mesh/RF24Mesh.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 /**
  * @file RF24Mesh.cpp
  *
- * Class definitions for RF24Mesh
+ * Class definitions for ESBMesh
  */
 
 #include "RF24Mesh.h"
 #include "RF24Mesh_config.h"
 #if defined(__linux) && !defined(__ARDUINO_X86__)
     #include <fstream>
 #endif
 
-RF24Mesh::RF24Mesh(RF24& _radio, RF24Network& _network) : radio(_radio), network(_network)
+template<class network_t, class radio_t>
+ESBMesh<network_t, radio_t>::ESBMesh(radio_t& _radio, network_t& _network) : radio(_radio), network(_network)
 {
     setCallback(NULL);
     meshStarted = false;
 #if !defined(MESH_NOMASTER)
     addrMemAllocated = false;
 #endif
 }
 
 /*****************************************************/
 
-bool RF24Mesh::begin(uint8_t channel, rf24_datarate_e data_rate, uint32_t timeout)
+template<class network_t, class radio_t>
+bool ESBMesh<network_t, radio_t>::begin(uint8_t channel, rf24_datarate_e data_rate, uint32_t timeout)
 {
     //delay(1); // Found problems w/SPIDEV & ncurses. Without this, getch() returns a stream of garbage
     if (meshStarted) {
         radio.stopListening();
     }
     meshStarted = true;
     if (!radio.begin())
@@ -53,15 +55,16 @@
     }
 
     return true;
 }
 
 /*****************************************************/
 
-uint8_t RF24Mesh::update()
+template<class network_t, class radio_t>
+uint8_t ESBMesh<network_t, radio_t>::update()
 {
     uint8_t type = network.update();
     if (mesh_address == MESH_DEFAULT_ADDRESS) return type;
 
 #if !defined(MESH_NOMASTER)
     if (type == NETWORK_REQ_ADDRESS) {
         doDHCP = 1;
@@ -96,25 +99,27 @@
 #endif //!NO_MASTER
 
     return type;
 }
 
 /*****************************************************/
 
-bool RF24Mesh::write(uint16_t to_node, const void* data, uint8_t msg_type, size_t size)
+template<class network_t, class radio_t>
+bool ESBMesh<network_t, radio_t>::write(uint16_t to_node, const void* data, uint8_t msg_type, size_t size)
 {
     if (mesh_address == MESH_DEFAULT_ADDRESS) return 0;
 
     RF24NetworkHeader header(to_node, msg_type);
     return network.write(header, data, size);
 }
 
 /*****************************************************/
 
-bool RF24Mesh::write(const void* data, uint8_t msg_type, size_t size, uint8_t nodeID)
+template<class network_t, class radio_t>
+bool ESBMesh<network_t, radio_t>::write(const void* data, uint8_t msg_type, size_t size, uint8_t nodeID)
 {
     if (mesh_address == MESH_DEFAULT_ADDRESS) return 0;
 
     int16_t toNode = 0;
     uint32_t lookupTimeout = millis() + MESH_WRITE_TIMEOUT;
     uint32_t retryDelay = 5;
 
@@ -128,44 +133,48 @@
         }
     }
     return write(toNode, data, msg_type, size);
 }
 
 /*****************************************************/
 
-void RF24Mesh::setChannel(uint8_t _channel)
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::setChannel(uint8_t _channel)
 {
     radio.stopListening();
     radio.setChannel(_channel);
     radio.startListening();
 }
 
 /*****************************************************/
 
-void RF24Mesh::setChild(bool allow)
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::setChild(bool allow)
 {
     network.networkFlags = allow ? network.networkFlags & ~FLAG_NO_POLL : network.networkFlags | FLAG_NO_POLL;
 }
 
 /*****************************************************/
 
-bool RF24Mesh::checkConnection()
+template<class network_t, class radio_t>
+bool ESBMesh<network_t, radio_t>::checkConnection()
 {
     // getAddress() doesn't use auto-ack; do a double-check to manually retry 1 more time
     if (getAddress(_nodeID) < 1) {
         if (getAddress(_nodeID) < 1) {
             return false;
         }
     }
     return true;
 }
 
 /*****************************************************/
 
-int16_t RF24Mesh::getAddress(uint8_t nodeID)
+template<class network_t, class radio_t>
+int16_t ESBMesh<network_t, radio_t>::getAddress(uint8_t nodeID)
 { // Master will return and send 00 address for a nodeID with address 0, -1 if not found
 
     //if (nodeID == _nodeID) return mesh_address;
     if (!nodeID) return 0;
     if (mesh_address == MESH_DEFAULT_ADDRESS) return -2;
 
 // Lets say 0 if nodeID 0,  -1 if write failed or timed out, -2 if not found in list or address is default,
@@ -194,15 +203,16 @@
         return address;
     }
     return -1;
 }
 
 /*****************************************************/
 
-int16_t RF24Mesh::getNodeID(uint16_t address)
+template<class network_t, class radio_t>
+int16_t ESBMesh<network_t, radio_t>::getNodeID(uint16_t address)
 {
     if (address == MESH_BLANK_ID) return _nodeID;
     if (address == 0) return 0;
     if (mesh_address == MESH_DEFAULT_ADDRESS) return -2;
 
 #if !defined(MESH_NOMASTER)
     if (!mesh_address) { //Master Node
@@ -227,50 +237,54 @@
         return ID;
     }
     return -1;
 }
 
 /*****************************************************/
 
-uint8_t RF24Mesh::getLevel(uint16_t address)
+template<class network_t, class radio_t>
+uint8_t ESBMesh<network_t, radio_t>::getLevel(uint16_t address)
 {
     uint8_t count = 0;
     while (address) {
         address >>= 3;
         count++;
     }
     return count;
 }
 
 /*****************************************************/
 
-void RF24Mesh::beginDefault()
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::beginDefault()
 {
     radio.stopListening();
     network.begin(MESH_DEFAULT_ADDRESS);
     mesh_address = MESH_DEFAULT_ADDRESS;
 }
 
 /*****************************************************/
 
-bool RF24Mesh::releaseAddress()
+template<class network_t, class radio_t>
+bool ESBMesh<network_t, radio_t>::releaseAddress()
 {
     if (mesh_address == MESH_DEFAULT_ADDRESS) return 0;
 
     RF24NetworkHeader header(00, MESH_ADDR_RELEASE);
     if (network.write(header, 0, 0)) {
         beginDefault();
         return 1;
     }
     return 0;
 }
 
 /*****************************************************/
 
-uint16_t RF24Mesh::renewAddress(uint32_t timeout)
+template<class network_t, class radio_t>
+uint16_t ESBMesh<network_t, radio_t>::renewAddress(uint32_t timeout)
 {
     if (radio.available()) network.update();
 
     uint8_t reqCounter = 0;
     uint8_t totalReqs = 0;
 
     beginDefault();
@@ -291,15 +305,16 @@
         totalReqs = totalReqs % 10;
     }
     return mesh_address;
 }
 
 /*****************************************************/
 
-bool RF24Mesh::requestAddress(uint8_t level)
+template<class network_t, class radio_t>
+bool ESBMesh<network_t, radio_t>::requestAddress(uint8_t level)
 {
     RF24NetworkHeader header(MESH_MULTICAST_ADDRESS, NETWORK_POLL);
     //Find another radio, starting with level 0 multicast
     IF_MESH_DEBUG(printf_P(PSTR("%u: MSH Poll\n"), millis()));
     network.multicast(header, 0, 0, level);
 
     uint32_t timr = millis();
@@ -393,30 +408,33 @@
         }
     }
     return 1;
 }
 
 /*****************************************************/
 
-void RF24Mesh::setNodeID(uint8_t nodeID)
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::setNodeID(uint8_t nodeID)
 {
     _nodeID = nodeID;
 }
 
 /*****************************************************/
 #if !defined(MESH_NOMASTER)
 
-void RF24Mesh::setStaticAddress(uint8_t nodeID, uint16_t address)
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::setStaticAddress(uint8_t nodeID, uint16_t address)
 {
     setAddress(nodeID, address);
 }
 
 /*****************************************************/
 
-void RF24Mesh::setAddress(uint8_t nodeID, uint16_t address, bool searchBy)
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::setAddress(uint8_t nodeID, uint16_t address, bool searchBy)
 {
     //Look for the node in the list
     for (uint8_t i = 0; i < addrListTop; i++) {
         if (searchBy == false) {
             if (addrList[i].nodeID == nodeID) {
                 addrList[i].address = address;
     #if defined(__linux) && !defined(__ARDUINO_X86__)
@@ -445,15 +463,16 @@
     #if defined(__linux) && !defined(__ARDUINO_X86__)
     saveDHCP();
     #endif
 }
 
 /*****************************************************/
 
-void RF24Mesh::loadDHCP()
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::loadDHCP()
 {
 
     #if defined(__linux) && !defined(__ARDUINO_X86__)
     std::ifstream infile("dhcplist.txt", std::ifstream::binary);
     if (!infile) return;
 
     infile.seekg(0, infile.end);
@@ -468,29 +487,31 @@
     }
     infile.close();
     #endif
 }
 
 /*****************************************************/
 
-void RF24Mesh::saveDHCP()
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::saveDHCP()
 {
     #if defined(__linux) && !defined(__ARDUINO_X86__)
     std::ofstream outfile("dhcplist.txt", std::ofstream::binary | std::ofstream::trunc);
 
     for (int i = 0; i < addrListTop; i++) {
         outfile.write((char*)&addrList[i], sizeof(addrListStruct));
     }
     outfile.close();
     #endif // __linux & not X86
 }
 
 /*****************************************************/
 
-void RF24Mesh::DHCP()
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::DHCP()
 {
     if (doDHCP)
         doDHCP = false;
     else
         return;
 
     RF24NetworkHeader header;
@@ -572,14 +593,21 @@
     } // end for
 }
 
 /*****************************************************/
 
 #endif // !MESH_NOMASTER
 
-void RF24Mesh::setCallback(void (*meshCallback)(void))
+template<class network_t, class radio_t>
+void ESBMesh<network_t, radio_t>::setCallback(void (*meshCallback)(void))
 {
 
     this->meshCallback = meshCallback;
 }
 
 /*****************************************************/
+
+// ensure the compiler is aware of the possible datatype for the template class
+template class ESBMesh<ESBNetwork<RF24>, RF24>;
+#if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840)
+template class ESBMesh<ESBNetwork<nrf_to_nrf>, nrf_to_nrf>;
+#endif
```

### Comparing `pyrf24-0.2.2/RF24Mesh/RF24Mesh.h` & `pyrf24-0.2.3/RF24Mesh/RF24Mesh.h`

 * *Files 8% similar despite different names*

```diff
@@ -37,44 +37,71 @@
 #if defined(__linux) && !defined(__ARDUINO_X86__) && !defined(USE_RF24_LIB_SRC)
     #include <RF24/RF24.h>
     #include <RF24Network/RF24Network.h>
     #define RF24_LINUX
 #else
     #include <RF24.h>
     #include <RF24Network.h>
+    #if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840)
+        #include <nrf_to_nrf.h>
+    #endif
 #endif
 
 #include <stddef.h>
 #include <stdint.h>
 
 class RF24;
-class RF24Network;
+#if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840) || defined(ARDUINO_ARCH_NRF52833)
+class nrf_to_nrf;
+#endif
+
+template<class radio_t>
+class ESBNetwork;
 
-class RF24Mesh
+/**
+ * @tparam network_t The `network` object's type. Defaults to `RF24Network` for legacy behavior.
+ * This new abstraction is really meant for using the nRF52840 SoC as a drop-in replacement
+ * for the nRF24L01 radio. For more detail, see the
+ * [nrf_to_nrf Arduino library](https://github.com/TMRh20/nrf_to_nrf).
+ * @tparam radio_t The `radio` object's type. Defaults to `RF24` for legacy behavior.
+ * This new abstraction is really meant for using the nRF52840 SoC as a drop-in replacement
+ * for the nRF24L01 radio. For more detail, see the
+ * [nrf_to_nrf Arduino library](https://github.com/TMRh20/nrf_to_nrf).
+ */
+template<class network_t = ESBNetwork<RF24>, class radio_t = RF24>
+class ESBMesh
 {
     /**
      * @name RF24Mesh
      *
      * The mesh library and class documentation is currently in active development and usage may change.
      */
     /**@{*/
 
 public:
     /**
-     * Construct the mesh:
-     *
+     * Construct the mesh.
+     * 
+     * v2.0 supports a backward compatible constructor:
      * @code
      * RF24 radio(7, 8);
      * RF24Network network(radio);
-     * RF24Mesh mesh(radio, network);
+     * RF24Mesh mesh(radio, network); // for nRF24L01
+     *
+     * nrf_to_nrf radio1;
+     * RF52Network network1(radio1);
+     * RF52Mesh mesh1(network1, radio1); // for nRF52xxx family
      * @endcode
+     * 
+     * @see v2.0 supports [nrf_to_nrf Arduino library](https://github.com/TMRh20/nrf_to_nrf)
+     * for nrf52 chips' internal radio.
      * @param _radio The underlying radio driver instance
      * @param _network The underlying network instance
      */
-    RF24Mesh(RF24& _radio, RF24Network& _network);
+    ESBMesh(radio_t& _radio, network_t& _network);
 
     /**
      * Call this in setup() to configure the mesh and request an address.  <br>
      *
      * @code mesh.begin(); @endcode
      * This may take a few moments to complete.
      *
@@ -106,15 +133,15 @@
      * @return True if success; false if failed
      */
     bool write(const void* data, uint8_t msg_type, size_t size, uint8_t nodeID = 0);
 
     /**
      * Set a unique @ref _nodeID "nodeID" for this node.
      *
-     * This needs to be called before RF24Mesh::begin(). The parameter value passed can be fetched
+     * This needs to be called before ESBMesh::begin(). The parameter value passed can be fetched
      * via serial connection, EEPROM, etc when configuring a large number of nodes.
      * @note If using RF24Gateway and/or RF24Ethernet, nodeIDs 0 & 1 are used by the master node.
      * @param nodeID Can be any unique value ranging from 1 to 255 (reserving 0 for the master node).
      */
     void setNodeID(uint8_t nodeID);
 
     /**
@@ -134,15 +161,15 @@
 
 #if !defined(MESH_NOMASTER)
     /**
      * This is only to be used on the master node because it manages allocation of network addresses
      * for any requesting (non-master) node's ID, similar to DHCP.
      *
      * @warning On master nodes, It is required to call this function immediately after calling
-     * RF24Mesh::update() to ensure address requests are handled appropriately.
+     * ESBMesh::update() to ensure address requests are handled appropriately.
      */
     void DHCP();
 
 #endif
 
     /**@}*/
     /**
@@ -283,15 +310,15 @@
      * `0`.
      */
     uint8_t _nodeID;
 
 #if !defined(MESH_NOMASTER)
     /**
      * @brief A struct for storing a  @ref _nodeID "nodeID" and an address in a single element of
-     * the RF24Mesh::addrList array.
+     * the ESBMesh::addrList array.
      *
      * @note This array only exists on the mesh network's master node.
      */
     typedef struct
     {
         /** @brief The @ref _nodeID "nodeID" of an network node (child) */
         uint8_t nodeID;
@@ -314,16 +341,16 @@
     addrListStruct* addrList;
     /** @brief The number of entries in the addrListStruct of assigned addresses. */
     uint8_t addrListTop;
 #endif
     /**@}*/
 
 private:
-    RF24& radio;
-    RF24Network& network;
+    radio_t& radio;
+    network_t& network;
 
     /** Function pointer for customized callback usage in long running algorithms. */
     void (*meshCallback)(void);
 
     /** Actual requesting of the address once a contact node is discovered or supplied **/
     bool requestAddress(uint8_t level);
 
@@ -339,14 +366,31 @@
     /** A flag asserted in begin() after putting the radio in TX mode. */
     bool meshStarted;
     /** Returns the number of octal digits in the specified address. */
     uint8_t getLevel(uint16_t address);
 };
 
 /**
+ * A type definition of the template class `ESBMesh` to maintain backward compatibility.
+ * 
+ * ```.cpp
+ * RF24 radio(7, 8);
+ * RF24Network network(radio);
+ * 
+ * RF24Mesh mesh(radio, network);
+ * // is equivalent to
+ * ESBMesh<ESBNetwork<RF24>, RF24> mesh(radio, network);
+ * ```
+ */
+typedef ESBMesh<ESBNetwork<RF24>, RF24> RF24Mesh;
+#if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840) || defined(ARDUINO_ARCH_NRF52833)
+typedef ESBMesh<ESBNetwork<nrf_to_nrf>, nrf_to_nrf> RF52Mesh;
+#endif
+
+/**
  * @example RF24Mesh_Example.ino
  * <b> Arduino Example Sketch </b><br>
  * This example sketch shows how to manually configure a node via RF24Mesh, and send data to the
  * master node.
  * The nodes will refresh their network address as soon as a single write fails. This allows the
  * nodes to change position in relation to each other and the master node.
  */
```

### Comparing `pyrf24-0.2.2/RF24Mesh/RF24Mesh_config.h` & `pyrf24-0.2.3/RF24Mesh/RF24Mesh_config.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/AutoConfig_RF24_DRIVER.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/CPackInfo.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/CPackInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/Cache.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/CompilerWarnings.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/GetLibInfo.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/GetLibInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/PreventInSourceBuilds.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/StandardProjectSettings.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/detectCPU.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/detectCPU.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Mesh/cmake/enableNcursesExample.cmake` & `pyrf24-0.2.3/RF24Mesh/cmake/enableNcursesExample.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/CMakeLists.txt` & `pyrf24-0.2.3/RF24Network/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/LICENSE` & `pyrf24-0.2.3/RF24Network/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/RF24Network.cpp` & `pyrf24-0.2.3/RF24Network/RF24Network.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     #include <iostream>
     #include <algorithm>
     #if !defined(USE_RF24_LIB_SRC)
         #include <RF24/RF24.h>
     #endif
 #else
     #include "RF24.h"
+    #if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840)
+        #include <nrf_to_nrf.h>
+    #endif
 #endif
 #include "RF24Network.h"
 #if defined(USE_RF24_LIB_SRC)
     #include <RF24.h>
 #endif
 
 #if defined(ENABLE_SLEEP_MODE) && defined(ESP8266)
@@ -41,36 +44,38 @@
 volatile byte sleep_cycles_remaining;
 volatile bool wasInterrupted;
 #endif
 uint16_t RF24NetworkHeader::next_id = 1;
 
 #if defined(RF24_LINUX)
 /******************************************************************/
-
-RF24Network::RF24Network(RF24& _radio) : radio(_radio), frame_size(MAX_FRAME_SIZE)
+template<class radio_t>
+ESBNetwork<radio_t>::ESBNetwork(radio_t& _radio) : radio(_radio), frame_size(MAX_FRAME_SIZE)
 {
     networkFlags = 0;
     returnSysMsgs = 0;
     multicastRelay = 0;
 }
 #else
-RF24Network::RF24Network(RF24& _radio) : radio(_radio), next_frame(frame_queue)
+template<class radio_t>
+ESBNetwork<radio_t>::ESBNetwork(radio_t& _radio) : radio(_radio), next_frame(frame_queue)
 {
     #if !defined(DISABLE_FRAGMENTATION)
     frag_queue.message_buffer = &frag_queue_message_buffer[0];
     frag_ptr = &frag_queue;
     #endif
     networkFlags = 0;
     returnSysMsgs = 0;
     multicastRelay = 0;
 }
 #endif
 /******************************************************************/
 
-void RF24Network::begin(uint8_t _channel, uint16_t _node_address)
+template<class radio_t>
+void ESBNetwork<radio_t>::begin(uint8_t _channel, uint16_t _node_address)
 {
     if (!is_valid_address(_node_address))
         return;
 
     node_address = _node_address;
 
     if (!radio.isValid())
@@ -104,24 +109,26 @@
 
     radio.startListening();
 }
 
 #if defined ENABLE_NETWORK_STATS
 /******************************************************************/
 
-void RF24Network::failures(uint32_t* _fails, uint32_t* _ok)
+template<class radio_t>
+void ESBNetwork<radio_t>::failures(uint32_t* _fails, uint32_t* _ok)
 {
     *_fails = nFails;
     *_ok = nOK;
 }
 #endif
 
 /******************************************************************/
 
-uint8_t RF24Network::update(void)
+template<class radio_t>
+uint8_t ESBNetwork<radio_t>::update(void)
 {
 
     uint8_t returnVal = 0;
 
     uint32_t timeout = millis();
 
     while (radio.available()) {
@@ -143,25 +150,24 @@
         // Read the beginning of the frame as the header
         RF24NetworkHeader* header = (RF24NetworkHeader*)(&frame_buffer);
 
         // Throw it away if it's not a valid address or too small
         if (frame_size < sizeof(RF24NetworkHeader) || !is_valid_address(header->to_node) || !is_valid_address(header->from_node)) {
             continue;
         }
-
-        IF_SERIAL_DEBUG(printf_P(PSTR("%u: MAC Received " PRIPSTR
-                                      "\n\r"),
-                                 millis(), header->toString()));
+        //IF_SERIAL_DEBUG(printf_P(PSTR("MAC Received " PRIPSTR
+        //                              "\n\r"),
+        //                         header->toString()));
 #if defined(RF24_LINUX)
         if (frame_size) {
             IF_SERIAL_DEBUG_FRAGMENTATION_L2(printf_P(PSTR("%u: FRG Rcv frame size %i\n"), millis(), frame_size););
             IF_SERIAL_DEBUG_FRAGMENTATION_L2(printf_P(PSTR("%u: FRG Rcv frame "), millis()); const char* charPtr = reinterpret_cast<const char*>(frame_buffer); for (uint16_t i = 0; i < frame_size; i++) { printf_P(PSTR("%02X "), charPtr[i]); }; printf_P(PSTR("\n\r")));
         }
 #else
-        IF_SERIAL_DEBUG(const uint16_t* i = reinterpret_cast<const uint16_t*>(frame_buffer + sizeof(RF24NetworkHeader)); printf_P(PSTR("%u: NET message %04x\n\r"), millis(), *i));
+        IF_SERIAL_DEBUG(const uint16_t* i = reinterpret_cast<const uint16_t*>(frame_buffer + sizeof(RF24NetworkHeader)); printf_P(PSTR("NET message %04x\n\r"), *i));
 #endif
 
         returnVal = header->type;
         // Is this for us?
         if (header->to_node == node_address) {
             if (header->type == NETWORK_PING) {
                 continue;
@@ -177,15 +183,15 @@
             if (header->type == NETWORK_REQ_ADDRESS && node_address) {
                 header->from_node = node_address;
                 header->to_node = 0;
                 write(header->to_node, TX_NORMAL);
                 continue;
             }
             if ((returnSysMsgs && header->type > MAX_USER_DEFINED_HEADER_TYPE) || header->type == NETWORK_ACK) {
-                IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("%u: MAC System payload rcvd %d\n"), millis(), returnVal););
+                IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("MAC System payload rcvd %d\n"), returnVal););
                 if (header->type != NETWORK_FIRST_FRAGMENT && header->type != NETWORK_MORE_FRAGMENTS && header->type != EXTERNAL_DATA_TYPE && header->type != NETWORK_LAST_FRAGMENT) {
                     return returnVal;
                 }
             }
 
             if (enqueue(header) == 2) { //External data received
                 IF_SERIAL_DEBUG_MINIMAL(printf_P(PSTR("ret ext\n")););
@@ -210,15 +216,15 @@
                     }
                     continue;
                 }
 
                 uint8_t val = enqueue(header);
 
                 if (multicastRelay) {
-                    IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("%u: MAC FWD multicast frame from 0%o to level %u\n"), millis(), header->from_node, _multicast_level + 1););
+                    IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("MAC FWD multicast frame from 0%o to level %u\n"), header->from_node, _multicast_level + 1););
                     if ((node_address >> 3) != 0) {
                         // for all but the first level of nodes, those not directly connected to the master, we add the total delay per level
                         delayMicroseconds(600 * 4);
                     }
                     delayMicroseconds((node_address % 4) * 600);
                     write(levelToAddress(_multicast_level) << 3, USER_TX_MULTICAST);
                 }
@@ -243,15 +249,16 @@
     } // radio.available()
     return returnVal;
 }
 
 #if defined(RF24_LINUX)
 /******************************************************************/
 
-uint8_t RF24Network::enqueue(RF24NetworkHeader* header)
+template<class radio_t>
+uint8_t ESBNetwork<radio_t>::enqueue(RF24NetworkHeader* header)
 {
     uint8_t result = false;
 
     RF24NetworkFrame frame = RF24NetworkFrame(*header, frame_buffer + sizeof(RF24NetworkHeader), frame_size - sizeof(RF24NetworkHeader));
 
     bool isFragment = (frame.header.type == NETWORK_FIRST_FRAGMENT || frame.header.type == NETWORK_MORE_FRAGMENTS || frame.header.type == NETWORK_LAST_FRAGMENT);
 
@@ -324,15 +331,16 @@
     }
 
     return result;
 }
 
 /******************************************************************/
 
-bool RF24Network::appendFragmentToFrame(RF24NetworkFrame frame)
+template<class radio_t>
+bool ESBNetwork<radio_t>::appendFragmentToFrame(RF24NetworkFrame frame)
 {
 
     // This is the first of 2 or more fragments.
     if (frame.header.type == NETWORK_FIRST_FRAGMENT) {
         if (frameFragmentsCache.count(frame.header.from_node) != 0) {
             RF24NetworkFrame* f = &(frameFragmentsCache[frame.header.from_node]);
             //Already rcvd first frag
@@ -402,20 +410,21 @@
 
 /******************************************************************/
 
 #else // Not defined RF24_Linux
 
 /******************************************************************/
 
-uint8_t RF24Network::enqueue(RF24NetworkHeader* header)
+template<class radio_t>
+uint8_t ESBNetwork<radio_t>::enqueue(RF24NetworkHeader* header)
 {
     bool result = false;
     uint16_t message_size = frame_size - sizeof(RF24NetworkHeader);
 
-    IF_SERIAL_DEBUG(printf_P(PSTR("%u: NET Enqueue @%x\n"), millis(), next_frame - frame_queue));
+    IF_SERIAL_DEBUG(printf_P(PSTR("NET Enqueue @%x\n"), next_frame - frame_queue));
 
     #if !defined(DISABLE_FRAGMENTATION)
 
     bool isFragment = header->type == NETWORK_FIRST_FRAGMENT || header->type == NETWORK_MORE_FRAGMENTS || header->type == NETWORK_LAST_FRAGMENT;
 
     if (isFragment) {
 
@@ -427,16 +436,16 @@
             IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("queue first, total frags %d\n\r"), header->reserved););
             //Store the total size of the stored frame in message_size
             frag_queue.message_size = message_size;
             --frag_queue.header.reserved;
             IF_SERIAL_DEBUG_FRAGMENTATION_L2(for (int i = 0; i < frag_queue.message_size; i++) { printf_P(PSTR("%02x"), frag_queue.message_buffer[i]); });
             return true;
         }
-        else // NETWORK_MORE_FRAGMENTS
-            if (header->type == NETWORK_LAST_FRAGMENT || header->type == NETWORK_MORE_FRAGMENTS) {
+        // else if not first fragment
+        else if (header->type == NETWORK_LAST_FRAGMENT || header->type == NETWORK_MORE_FRAGMENTS) {
 
             if (frag_queue.message_size + message_size > MAX_PAYLOAD_SIZE) {
         #if defined(SERIAL_DEBUG_FRAGMENTATION) || defined(SERIAL_DEBUG_MINIMAL)
                 printf_P(PSTR("Drop frag %d Size exceeds max\n\r"), header->reserved);
         #endif
                 frag_queue.header.reserved = 0;
                 return false;
@@ -457,15 +466,15 @@
             }
             frag_queue.header.reserved = 0;
             frag_queue.header.type = header->reserved;
 
             IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("fq 3: %d\n"), frag_queue.message_size););
             IF_SERIAL_DEBUG_FRAGMENTATION_L2(for (int i = 0; i < frag_queue.message_size; i++) { printf_P(PSTR("%02X"), frag_queue.message_buffer[i]); });
 
-            //Frame assembly complete, copy to main buffer if OK
+            // Frame assembly complete, copy to main buffer if OK
             if (frag_queue.header.type == EXTERNAL_DATA_TYPE) {
                 return 2;
             }
         #if defined(DISABLE_USER_PAYLOADS)
             return 0;
         #endif
 
@@ -479,14 +488,15 @@
                 }
         #endif
                 IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("enq size %d\n"), frag_queue.message_size););
                 return true;
             }
             IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("Drop frag payload, queue full\n")););
             return false;
+
         } //If more or last fragments
     }
     else //else is not a fragment
     #endif // End fragmentation enabled
 
     // Copy the current frame into the frame queue
     #if !defined(DISABLE_FRAGMENTATION)
@@ -526,37 +536,40 @@
     return result;
 }
     #endif //USER_PAYLOADS_ENABLED
 
 #endif //End not defined RF24_Linux
 /******************************************************************/
 
-bool RF24Network::available(void)
+template<class radio_t>
+bool ESBNetwork<radio_t>::available(void)
 {
 #if defined(RF24_LINUX)
     return (!frame_queue.empty());
 #else
     // Are there frames on the queue for us?
     return (next_frame > frame_queue);
 #endif
 }
 
 /******************************************************************/
 
-uint16_t RF24Network::parent() const
+template<class radio_t>
+uint16_t ESBNetwork<radio_t>::parent() const
 {
     if (node_address == 0)
         return -1;
     else
         return parent_node;
 }
 
 /******************************************************************/
 
-uint16_t RF24Network::peek(RF24NetworkHeader& header)
+template<class radio_t>
+uint16_t ESBNetwork<radio_t>::peek(RF24NetworkHeader& header)
 {
     if (available()) {
 #if defined(RF24_LINUX)
         RF24NetworkFrame frame = frame_queue.front();
         memcpy(&header, &frame.header, sizeof(RF24NetworkHeader));
         return frame.message_size;
 #else
@@ -568,15 +581,16 @@
 #endif
     }
     return 0;
 }
 
 /******************************************************************/
 
-void RF24Network::peek(RF24NetworkHeader& header, void* message, uint16_t maxlen)
+template<class radio_t>
+void ESBNetwork<radio_t>::peek(RF24NetworkHeader& header, void* message, uint16_t maxlen)
 {
     if (available()) {
 #if defined(RF24_LINUX)
         RF24NetworkFrame frame = frame_queue.front();
         memcpy(&header, &(frame.header), sizeof(RF24NetworkHeader));
         if (maxlen > 0) {
             maxlen = rf24_min(frame.message_size, maxlen);
@@ -592,15 +606,16 @@
         }
 #endif
     }
 }
 
 /******************************************************************/
 
-uint16_t RF24Network::read(RF24NetworkHeader& header, void* message, uint16_t maxlen)
+template<class radio_t>
+uint16_t ESBNetwork<radio_t>::read(RF24NetworkHeader& header, void* message, uint16_t maxlen)
 {
     uint16_t bufsize = 0;
 
     // This function assumes that there is a frame in the queue.
     // Call `available()` before calling `read()`.
     //if (!available()) { return bufsize; }
 
@@ -625,17 +640,17 @@
 
     memcpy(&header, frame_queue, 8);
     memcpy(&bufsize, frame_queue + 8, 2);
 
     if (maxlen > 0) {
         maxlen = rf24_min(maxlen, bufsize);
         memcpy(message, frame_queue + 10, maxlen);
-        IF_SERIAL_DEBUG(printf_P(PSTR("%u: NET message size %d\n"), millis(), bufsize););
+        IF_SERIAL_DEBUG(printf_P(PSTR("NET message size %d\n"), bufsize););
 
-        IF_SERIAL_DEBUG(uint16_t len = maxlen; printf_P(PSTR("%u: NET message "), millis()); const uint8_t* charPtr = reinterpret_cast<const uint8_t*>(message); while (len--) { printf_P(PSTR("%02x "), charPtr[len]); } printf_P(PSTR("\n\r")));
+        IF_SERIAL_DEBUG(uint16_t len = maxlen; printf_P(PSTR("NET message ")); const uint8_t* charPtr = reinterpret_cast<const uint8_t*>(message); while (len--) { printf_P(PSTR("%02x "), charPtr[len]); } printf_P(PSTR("\n\r")));
     }
     next_frame -= bufsize + 10;
     uint8_t padding = 0;
     #if !defined(ARDUINO_ARCH_AVR)
     if ((padding = (bufsize + 10) % 4)) {
         padding = 4 - padding;
         next_frame -= padding;
@@ -647,56 +662,60 @@
 #endif // !defined(RF24_LINUX)
     return bufsize;
 }
 
 #if defined RF24NetworkMulticast
 /******************************************************************/
 
-bool RF24Network::multicast(RF24NetworkHeader& header, const void* message, uint16_t len, uint8_t level)
+template<class radio_t>
+bool ESBNetwork<radio_t>::multicast(RF24NetworkHeader& header, const void* message, uint16_t len, uint8_t level)
 {
     // Fill out the header
     header.to_node = NETWORK_MULTICAST_ADDRESS;
     header.from_node = node_address;
     return write(header, message, len, levelToAddress(level > 4 ? _multicast_level : level));
 }
 #endif
 
 /******************************************************************/
 
-bool RF24Network::write(RF24NetworkHeader& header, const void* message, uint16_t len)
+template<class radio_t>
+bool ESBNetwork<radio_t>::write(RF24NetworkHeader& header, const void* message, uint16_t len)
 {
     return write(header, message, len, NETWORK_AUTO_ROUTING);
 }
 
 /******************************************************************/
 
-bool RF24Network::write(RF24NetworkHeader& header, const void* message, uint16_t len, uint16_t writeDirect)
+template<class radio_t>
+bool ESBNetwork<radio_t>::write(RF24NetworkHeader& header, const void* message, uint16_t len, uint16_t writeDirect)
 {
 
 #if defined(DISABLE_FRAGMENTATION)
     frame_size = rf24_min(len + sizeof(RF24NetworkHeader), MAX_FRAME_SIZE);
     return _write(header, message, rf24_min(len, max_frame_payload_size), writeDirect);
 #else // !defined(DISABLE_FRAGMENTATION)
     if (len <= max_frame_payload_size) {
         //Normal Write (Un-Fragmented)
         frame_size = len + sizeof(RF24NetworkHeader);
         return _write(header, message, len, writeDirect);
     }
     //Check payload size
+
     if (len > MAX_PAYLOAD_SIZE) {
-        IF_SERIAL_DEBUG(printf_P(PSTR("%u: NET write message failed. Given 'len' %d is bigger than the MAX Payload size %i\n\r"), millis(), len, MAX_PAYLOAD_SIZE););
+        IF_SERIAL_DEBUG(printf_P(PSTR("NET write message failed. Given 'len' %d is bigger than the MAX Payload size %i\n\r"), len, MAX_PAYLOAD_SIZE););
         return false;
     }
 
     //Divide the message payload into chunks of max_frame_payload_size
     uint8_t fragment_id = (len % max_frame_payload_size != 0) + ((len) / max_frame_payload_size); //the number of fragments to send = ceil(len/max_frame_payload_size)
 
     uint8_t msgCount = 0;
 
-    IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("%u: FRG Total message fragments %d\n\r"), millis(), fragment_id););
+    IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("FRG Total message fragments %d\n\r"), fragment_id););
 
     if (header.to_node != NETWORK_MULTICAST_ADDRESS) {
         networkFlags |= FLAG_FAST_FRAG;
         radio.stopListening();
     }
 
     uint8_t retriesPerFrag = 0;
@@ -736,63 +755,64 @@
             fragment_id--;
             msgCount++;
         }
 
         //if(writeDirect != NETWORK_AUTO_ROUTING){ delay(2); } //Delay 2ms between sending multicast payloads
 
         if (!ok && retriesPerFrag >= 3) {
-            IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("%u: FRG TX with fragmentID '%d' failed after %d fragments. Abort.\n\r"), millis(), fragment_id, msgCount));
+            IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("FRG TX with fragmentID '%d' failed after %d fragments. Abort.\n\r"), fragment_id, msgCount));
             break;
         }
 
-        //Message was successful sent
-        IF_SERIAL_DEBUG_FRAGMENTATION_L2(printf_P(PSTR("%u: FRG message transmission with fragmentID '%d' successful.\n\r"), millis(), fragment_id));
+        // Message was successful sent
+        IF_SERIAL_DEBUG_FRAGMENTATION_L2(printf_P(PSTR("FRG message transmission with fragmentID '%d' successful.\n\r"), fragment_id));
     }
     header.type = type;
     if (networkFlags & FLAG_FAST_FRAG) {
         ok = radio.txStandBy(txTimeout);
         radio.startListening();
         radio.setAutoAck(0, 0);
     }
     networkFlags &= ~FLAG_FAST_FRAG;
 
-    //Return true if all the chunks where sent successfully
+    // Return true if all the chunks where sent successfully
+    IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("FRG total message fragments sent %i.\r\n"), msgCount););
 
-    IF_SERIAL_DEBUG_FRAGMENTATION(printf_P(PSTR("%u: FRG total message fragments sent %i.\r\n"), millis(), msgCount););
     if (!ok || fragment_id > 0) {
         return false;
     }
     return true;
 
 #endif //Fragmentation enabled
 }
 
 /******************************************************************/
 
-bool RF24Network::_write(RF24NetworkHeader& header, const void* message, uint16_t len, uint16_t writeDirect)
+template<class radio_t>
+bool ESBNetwork<radio_t>::_write(RF24NetworkHeader& header, const void* message, uint16_t len, uint16_t writeDirect)
 {
     // Fill out the header
     header.from_node = node_address;
 
     // Build the full frame to send
     memcpy(frame_buffer, &header, sizeof(RF24NetworkHeader));
 
-    IF_SERIAL_DEBUG(printf_P(PSTR("%u: NET Sending " PRIPSTR
-                                  "\n\r"),
-                             millis(), header.toString()));
+    //IF_SERIAL_DEBUG(printf_P(PSTR("NET Sending " PRIPSTR
+    //                              "\n\r"),
+    //                         header.toString()));
     if (len) {
 #if defined(RF24_LINUX)
         memcpy(frame_buffer + sizeof(RF24NetworkHeader), message, rf24_min(frame_size - sizeof(RF24NetworkHeader), len));
         IF_SERIAL_DEBUG(printf_P(PSTR("%u: FRG frame size %i\n"), millis(), frame_size););
         IF_SERIAL_DEBUG(printf_P(PSTR("%u: FRG frame "), millis()); const char* charPtr = reinterpret_cast<const char*>(frame_buffer); for (uint16_t i = 0; i < frame_size; i++) { printf_P(PSTR("%02X "), charPtr[i]); }; printf_P(PSTR("\n\r")));
 #else
 
         memcpy(frame_buffer + sizeof(RF24NetworkHeader), message, len);
 
-        IF_SERIAL_DEBUG(uint16_t tmpLen = len; printf_P(PSTR("%u: NET message "), millis()); const uint8_t* charPtr = reinterpret_cast<const uint8_t*>(message); while (tmpLen--) { printf_P(PSTR("%02x "), charPtr[tmpLen]); } printf_P(PSTR("\n\r")));
+        IF_SERIAL_DEBUG(uint16_t tmpLen = len; printf_P(PSTR("NET message ")); const uint8_t* charPtr = reinterpret_cast<const uint8_t*>(message); while (tmpLen--) { printf_P(PSTR("%02x "), charPtr[tmpLen]); } printf_P(PSTR("\n\r")));
 #endif
     }
 
     // If the user is trying to send it to himself
     /*if (header.to_node == node_address) {
     #if defined (RF24_LINUX)
         RF24NetworkFrame frame = RF24NetworkFrame(header, message, rf24_min(MAX_FRAME_SIZE - sizeof(RF24NetworkHeader), len));
@@ -815,15 +835,16 @@
         return write(writeDirect, sendType);
     }
     return write(header.to_node, TX_NORMAL);
 }
 
 /******************************************************************/
 
-bool RF24Network::write(uint16_t to_node, uint8_t sendType)
+template<class radio_t>
+bool ESBNetwork<radio_t>::write(uint16_t to_node, uint8_t sendType)
 {
     bool ok = false;
     bool isAckType = false;
     if (frame_buffer[6] > 64 && frame_buffer[6] < 192)
         isAckType = true;
 
     /*if( ( (frame_buffer[7] % 2) && frame_buffer[6] == NETWORK_MORE_FRAGMENTS) ){
@@ -834,23 +855,23 @@
     if (!is_valid_address(to_node))
         return false;
 
     //Load info into our conversion structure, and get the converted address info
     logicalToPhysicalStruct conversion = {to_node, sendType, 0};
     logicalToPhysicalAddress(&conversion);
 
-    IF_SERIAL_DEBUG(printf_P(PSTR("%u: MAC Sending to 0%o via 0%o on pipe %x\n\r"), millis(), to_node, conversion.send_node, conversion.send_pipe));
+    IF_SERIAL_DEBUG(printf_P(PSTR("MAC Sending to 0%o via 0%o on pipe %x\n\r"), to_node, conversion.send_node, conversion.send_pipe));
     /**Write it*/
     if (sendType == TX_ROUTED && conversion.send_node == to_node && isAckType) {
         delay(2);
     }
     ok = write_to_pipe(conversion.send_node, conversion.send_pipe, conversion.multicast);
 
     if (!ok) {
-        IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("%u: MAC Send fail to 0%o via 0%o on pipe %x\n\r"), millis(), to_node, conversion.send_node, conversion.send_pipe););
+        IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("MAC Send fail to 0%o via 0%o on pipe %x\n\r"), to_node, conversion.send_node, conversion.send_pipe););
     }
 
     if (sendType == TX_ROUTED && ok && conversion.send_node == to_node && isAckType) {
         // NETWORK_ACK messages are only sent by the last node in the route to a target node.
         // ie: Node 00 sends to node 011, node 01 will send the network ack to 00 upon delivery.
         // Any node receiving a NETWORK_ACK message will route it as a normal message.
 
@@ -863,16 +884,16 @@
         conversion.multicast = 0;
         logicalToPhysicalAddress(&conversion);
 
         //Write the data using the resulting physical address
         frame_size = sizeof(RF24NetworkHeader);
         write_to_pipe(conversion.send_node, conversion.send_pipe, conversion.multicast);
 
-        //dynLen=0;
-        IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("%u: MAC Route OK to 0%o ACK sent to 0%o\n"), millis(), to_node, header->from_node););
+        // dynLen=0;
+        IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("MAC Route OK to 0%o ACK sent to 0%o\n"), to_node, header->from_node););
     }
 
     if (ok && conversion.send_node != to_node && (sendType == TX_NORMAL || sendType == USER_TX_TO_LOGICAL_ADDRESS) && isAckType) {
         // Now, continue listening
         if (networkFlags & FLAG_FAST_FRAG) {
             radio.txStandBy(txTimeout);
             networkFlags &= ~FLAG_FAST_FRAG;
@@ -882,15 +903,15 @@
         uint32_t reply_time = millis();
 
         while (update() != NETWORK_ACK) {
 #if defined(RF24_LINUX)
             delayMicroseconds(900);
 #endif
             if (millis() - reply_time > routeTimeout) {
-                IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("%u: MAC Network ACK fail from 0%o via 0%o on pipe %x\n\r"), millis(), to_node, conversion.send_node, conversion.send_pipe););
+                IF_SERIAL_DEBUG_ROUTING(printf_P(PSTR("MAC Network ACK fail from 0%o via 0%o on pipe %x\n\r"), to_node, conversion.send_node, conversion.send_pipe););
                 ok = false;
                 break;
             }
         }
     }
     if (!(networkFlags & FLAG_FAST_FRAG)) {
         // Now, continue listening
@@ -906,15 +927,16 @@
     }
 #endif
     return ok;
 }
 
 /******************************************************************/
 
-void RF24Network::logicalToPhysicalAddress(logicalToPhysicalStruct* conversionInfo)
+template<class radio_t>
+void ESBNetwork<radio_t>::logicalToPhysicalAddress(logicalToPhysicalStruct* conversionInfo)
 {
 
     //Create pointers so this makes sense.. kind of
     //We take in the to_node(logical) now, at the end of the function, output the send_node(physical) address, etc.
     //back to the original memory address that held the logical information.
     uint16_t* to_node = &conversionInfo->send_node;
     uint8_t* directTo = &conversionInfo->send_pipe;
@@ -950,15 +972,16 @@
 
     *to_node = pre_conversion_send_node;
     *directTo = pre_conversion_send_pipe;
 }
 
 /********************************************************/
 
-bool RF24Network::write_to_pipe(uint16_t node, uint8_t pipe, bool multicast)
+template<class radio_t>
+bool ESBNetwork<radio_t>::write_to_pipe(uint16_t node, uint8_t pipe, bool multicast)
 {
     bool ok = false;
 
     // Open the correct pipe for writing.
     // First, stop listening so we can talk
     if (!(networkFlags & FLAG_FAST_FRAG)) {
         radio.stopListening();
@@ -994,37 +1017,40 @@
     //snprintf_P(buffer,sizeof(buffer),PSTR("id %04x from 0%o to 0%o type %c"),id,from_node,to_node,type);
     sprintf_P(buffer, PSTR("id %u from 0%o to 0%o type %d"), id, from_node, to_node, type);
     return buffer;
 }
 
 /******************************************************************/
 
-bool RF24Network::is_direct_child(uint16_t node)
+template<class radio_t>
+bool ESBNetwork<radio_t>::is_direct_child(uint16_t node)
 {
     // A direct child of ours has the same low numbers as us, and only
     // one higher number.
     //
     // e.g. node 0234 is a direct child of 034, and node 01234 is a
     // descendant but not a direct child
 
     // Does it only have ONE more level than us?
     uint16_t child_node_mask = (~node_mask) << 3;
     return (node & child_node_mask) == 0;
 }
 
 /******************************************************************/
 
-bool RF24Network::is_descendant(uint16_t node)
+template<class radio_t>
+bool ESBNetwork<radio_t>::is_descendant(uint16_t node)
 {
     return (node & node_mask) == node_address;
 }
 
 /******************************************************************/
 
-void RF24Network::setup_address(void)
+template<class radio_t>
+void ESBNetwork<radio_t>::setup_address(void)
 {
     // First, establish the node_mask
     uint16_t node_mask_check = 0xFFFF;
 #if defined(RF24NetworkMulticast)
     uint8_t count = 0;
 #endif
 
@@ -1060,15 +1086,16 @@
     //  IF_SERIAL_DEBUG_MINIMAL(Serial.print(node_address,OCT));
     //  IF_SERIAL_DEBUG_MINIMAL(Serial.print(F(" parent=")));
     //  IF_SERIAL_DEBUG_MINIMAL(Serial.println(parent_node,OCT));
 }
 
 /******************************************************************/
 
-uint16_t RF24Network::addressOfPipe(uint16_t node, uint8_t pipeNo)
+template<class radio_t>
+uint16_t ESBNetwork<radio_t>::addressOfPipe(uint16_t node, uint8_t pipeNo)
 {
     //Say this node is 013 (1011), mask is 077 or (00111111)
     //Say we want to use pipe 3 (11)
     //6 bits in node mask, so shift pipeNo 6 times left and | into address
     uint16_t m = node_mask >> 3;
     uint8_t i = 0;
 
@@ -1077,24 +1104,26 @@
         i++;     //Count the # of increments
     }
     return node | (pipeNo << i);
 }
 
 /******************************************************************/
 
-uint16_t RF24Network::direct_child_route_to(uint16_t node)
+template<class radio_t>
+uint16_t ESBNetwork<radio_t>::direct_child_route_to(uint16_t node)
 {
     // Presumes that this is in fact a child!!
     uint16_t child_mask = (node_mask << 3) | 0x07;
     return node & child_mask;
 }
 
 /******************************************************************/
 
-bool RF24Network::is_valid_address(uint16_t node)
+template<class radio_t>
+bool ESBNetwork<radio_t>::is_valid_address(uint16_t node)
 {
     bool result = true;
     if (node == NETWORK_MULTICAST_ADDRESS || node == 010) {
         return result;
     }
     uint8_t count = 0;
 #if defined(SERIAL_DEBUG_MINIMAL)
@@ -1117,40 +1146,43 @@
     }
     return result;
 }
 
 #if defined(RF24NetworkMulticast)
 /******************************************************************/
 
-void RF24Network::multicastLevel(uint8_t level)
+template<class radio_t>
+void ESBNetwork<radio_t>::multicastLevel(uint8_t level)
 {
     _multicast_level = level;
     radio.stopListening();
     radio.openReadingPipe(0, pipe_address(levelToAddress(level), 0));
     radio.startListening();
 }
 
 /******************************************************************/
 
-uint16_t RF24Network::levelToAddress(uint8_t level)
+template<class radio_t>
+uint16_t ESBNetwork<radio_t>::levelToAddress(uint8_t level)
 {
 
     uint16_t levelAddr = 1;
     if (level)
         levelAddr = levelAddr << ((level - 1) * 3);
     else
         return 0;
 
     return levelAddr;
 }
 
 #endif // !defined(RF24NetworkMulticast)
 /******************************************************************/
 
-uint64_t RF24Network::pipe_address(uint16_t node, uint8_t pipe)
+template<class radio_t>
+uint64_t ESBNetwork<radio_t>::pipe_address(uint16_t node, uint8_t pipe)
 {
 
     static uint8_t address_translation[] = {0xc3, 0x3c, 0x33, 0xce, 0x3e, 0xe3, 0xec};
     uint64_t result = 0xCCCCCCCCCCLL;
     uint8_t* out = reinterpret_cast<uint8_t*>(&result);
 
     // Translate the address to use our optimally chosen radio address bytes
@@ -1171,16 +1203,15 @@
     if (pipe != 0 || !node)
 #endif
         out[0] = address_translation[pipe];
 #if defined(RF24NetworkMulticast)
     else
         out[1] = address_translation[count - 1];
 #endif
-
-    IF_SERIAL_DEBUG(uint32_t* top = reinterpret_cast<uint32_t*>(out + 1); printf_P(PSTR("%u: NET Pipe %i on node 0%o has address %x%x\n\r"), millis(), pipe, node, *top, *out));
+    IF_SERIAL_DEBUG(uint32_t* top = reinterpret_cast<uint32_t*>(out + 1); printf_P(PSTR("NET Pipe %i on node 0%o has address %x%x\n\r"), pipe, node, *top, *out));
 
     return result;
 }
 
 /************************ Sleep Mode ******************************************/
 
 #if defined ENABLE_SLEEP_MODE
@@ -1194,15 +1225,16 @@
 }
 
 ISR(WDT_vect)
 {
     --sleep_cycles_remaining;
 }
 
-bool RF24Network::sleepNode(unsigned int cycles, int interruptPin, uint8_t INTERRUPT_MODE)
+template<class radio_t>
+bool ESBNetwork<radio_t>::sleepNode(unsigned int cycles, int interruptPin, uint8_t INTERRUPT_MODE)
 {
     sleep_cycles_remaining = cycles;
     set_sleep_mode(SLEEP_MODE_PWR_DOWN); // sleep mode is set here
     sleep_enable();
     if (interruptPin != 255) {
         wasInterrupted = false; //Reset Flag
         //LOW,CHANGE, FALLING, RISING correspond with the values 0,1,2,3 respectively
@@ -1229,15 +1261,16 @@
     WDTCR &= ~_BV(WDIE);
         #else
     WDTCSR &= ~_BV(WDIE);
         #endif
     return !wasInterrupted;
 }
 
-void RF24Network::setup_watchdog(uint8_t prescalar)
+template<class radio_t>
+void ESBNetwork<radio_t>::setup_watchdog(uint8_t prescalar)
 {
 
     uint8_t wdtcsr = prescalar & 7;
     if (prescalar & 8)
         wdtcsr |= _BV(WDP3);
     MCUSR &= ~_BV(WDRF); // Clear the WD System Reset Flag
 
@@ -1248,7 +1281,13 @@
     WDTCSR = _BV(WDCE) | _BV(WDE);           // Write the WD Change enable bit to enable changing the prescaler and enable system reset
     WDTCSR = _BV(WDCE) | wdtcsr | _BV(WDIE); // Write the prescalar bits (how long to sleep, enable the interrupt to wake the MCU
         #endif
 }
 
     #endif // not ATTiny
 #endif     // Enable sleep mode
+
+// ensure the compiler is aware of the possible datatype for the template class
+template class ESBNetwork<RF24>;
+#if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840) || defined(ARDUINO_ARCH_NRF52833)
+template class ESBNetwork<nrf_to_nrf>;
+#endif
```

### Comparing `pyrf24-0.2.2/RF24Network/RF24Network.h` & `pyrf24-0.2.3/RF24Network/RF24Network.h`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,17 @@
  * This flag (when asserted in RF24Network::networkFlags) prevents a node from responding to
  * mesh nodes looking to connect to the network. Calling RF24Mesh::setChild() uses this flag
  * accordingly.
  */
 #define FLAG_NO_POLL 8
 
 class RF24;
+#if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840) || defined(ARDUINO_ARCH_NRF52833)
+class nrf_to_nrf;
+#endif
 
 /**
  * Header which is sent with each message
  *
  * The frame put over the air consists of this header and a message
  *
  * Headers are addressed to the appropriate node, and the network forwards them on to their final destination.
@@ -349,15 +352,15 @@
     }
 #endif
 #if defined(DOXYGEN_FORCED) || !defined(RF24_LINUX)
     /**
      * **Constructor for Arduino/AVR/etc. platforms** - create a network frame with data
      * Frames are constructed and handled differently on Arduino/AVR and Linux devices (`#if defined RF24_LINUX`)
      *
-     * @see RF24Network.frag_ptr
+     * @see ESBNetwork.frag_ptr
      * @param _header The RF24Network header to be stored in the frame
      * @param _message_size The size of the 'message' or data
      *
      * Frames are used internally and by external systems. See RF24NetworkHeader.
      */
     RF24NetworkFrame(RF24NetworkHeader& _header, uint16_t _message_size) : header(_header), message_size(_message_size)
     {
@@ -366,32 +369,50 @@
 };
 
 /**
  * 2014-2021 - Optimized Network Layer for RF24 Radios
  *
  * This class implements an OSI Network Layer using nRF24L01(+) radios driven
  * by RF24 library.
+ *
+ * @tparam radio_t The `radio` object's type. Defaults to `RF24` for legacy behavior.
+ * This new abstraction is really meant for using the nRF52840 SoC as a drop-in replacement
+ * for the nRF24L01 radio. For more detail, see the
+ * [nrf_to_nrf Arduino library](https://github.com/TMRh20/nrf_to_nrf).
  */
-class RF24Network
+template<class radio_t = RF24>
+class ESBNetwork
 {
 
     /**
      * @name Primary Interface
      *
      *  These are the main methods you need to operate the network
      */
     /**@{*/
 
 public:
     /**
      * Construct the network
      *
+     * v2.0 supports a backward compatible constructor:
+     * @code
+     * RF24 radio(7, 8);
+     * RF24Network network(radio); // for nRF24L01
+     *
+     * nrf_to_nrf radio1;
+     * RF52Network network(radio1); // for nRF52xxx family
+     * @endcode
+     * 
+     * @see v2.0 supports [nrf_to_nrf Arduino library](https://github.com/TMRh20/nrf_to_nrf)
+     * for nrf52 chips' internal radio.
+     * 
      * @param _radio The underlying radio driver instance
      */
-    RF24Network(RF24& _radio);
+    ESBNetwork(radio_t& _radio);
 
     /**
      * Bring up the network using the current radio frequency/channel.
      * Calling begin brings up the network, and configures the address, which designates the
      * location of the node within [RF24Network topology](md_docs_tuning.html).
      *
      * @note Node addresses are specified in Octal format, see
@@ -688,15 +709,15 @@
      * Maintained for backwards compatibility
      */
     /**@{*/
 
     /**
      * Bring up the network on a specific radio frequency/channel.
      * @deprecated Use `RF24::setChannel()` to configure the radio channel.
-     * Use RF24Network::begin(uint16_t _node_address) to set the node address.
+     * Use ESBNetwork::begin(uint16_t _node_address) to set the node address.
      *
      * **Example 1:** Begin on channel 90 with address 0 (master node)
      * @code
      * network.begin(90, 0);
      * @endcode
      * **Example 2:** Begin on channel 90 with address 01 (child of master)
      * @code
@@ -907,15 +928,15 @@
     /* Returns true if the given logical address (`node` parameter) is a descendent of the current node; otherwise returns false. */
     bool is_descendant(uint16_t node);
     /* Returns a logical address for the first child en route to a child node */
     uint16_t direct_child_route_to(uint16_t node);
 
     /***********************************************************************/
 
-    RF24& radio; /** Underlying radio driver, provides link/physical layers */
+    radio_t& radio; /** Underlying radio driver, provides link/physical layers */
 
     uint8_t frame_size;                                                                            /* The outgoing frame's total size including the header info. Ranges [8, MAX_PAYLOAD_SIZE] */
     const static unsigned int max_frame_payload_size = MAX_FRAME_SIZE - sizeof(RF24NetworkHeader); /* always 24 bytes to compensate for the frame's header */
 
 #if defined(RF24_LINUX)
     std::queue<RF24NetworkFrame> frame_queue;
     std::map<uint16_t, RF24NetworkFrame> frameFragmentsCache;
@@ -935,15 +956,15 @@
     uint8_t frag_queue_message_buffer[MAX_PAYLOAD_SIZE]; //frame size + 1
     #endif
 
 #endif // Linux/Not Linux
 
     uint16_t parent_node; /** Our parent's node address */
     uint8_t parent_pipe;  /** The pipe our parent uses to listen to us */
-    uint16_t node_mask;   /** The bits which contain signfificant node address information */
+    uint16_t node_mask;   /** The bits which contain significant node address information */
 
     /* Given the Logical node address & a pipe number, this returns the Physical address assigned to the radio's pipes. */
     uint64_t pipe_address(uint16_t node, uint8_t pipe);
 
 #if defined ENABLE_NETWORK_STATS
     uint32_t nFails;
     uint32_t nOK;
@@ -954,14 +975,30 @@
     uint16_t levelToAddress(uint8_t level);
 #endif
 
     /** @} */
 };
 
 /**
+ * A type definition of the template class `ESBNetwork` to maintain backward compatibility.
+ *
+ * ```.cpp
+ * RF24 radio(7, 8);
+ *
+ * RF24Network network(radio);
+ * // is equivalent to
+ * ESBNetwork<RF24> network(radio);
+ * ```
+ */
+typedef ESBNetwork<RF24> RF24Network;
+#if defined(ARDUINO_ARCH_NRF52) || defined(ARDUINO_ARCH_NRF52840) || defined(ARDUINO_ARCH_NRF52833)
+typedef ESBNetwork<nrf_to_nrf> RF52Network;
+#endif
+
+/**
  * @example helloworld_tx.ino
  *
  * Simplest possible example of using RF24Network. Put this sketch
  * on one node, and helloworld_rx.pde on the other. Tx will send
  * Rx a nice message every 2 seconds which rx will print out for us.
  */
```

### Comparing `pyrf24-0.2.2/RF24Network/RF24Network_config.h` & `pyrf24-0.2.3/RF24Network/RF24Network_config.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake` & `pyrf24-0.2.3/RF24Network/cmake/AutoConfig_RF24_DRIVER.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/CPackInfo.cmake` & `pyrf24-0.2.3/RF24Network/cmake/CPackInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/Cache.cmake` & `pyrf24-0.2.3/RF24Network/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/CompilerWarnings.cmake` & `pyrf24-0.2.3/RF24Network/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/GetLibInfo.cmake` & `pyrf24-0.2.3/RF24Network/cmake/GetLibInfo.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/PreventInSourceBuilds.cmake` & `pyrf24-0.2.3/RF24Network/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/StandardProjectSettings.cmake` & `pyrf24-0.2.3/RF24Network/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/RF24Network/cmake/detectCPU.cmake` & `pyrf24-0.2.3/RF24Network/cmake/detectCPU.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/cmake/using_flags.cmake` & `pyrf24-0.2.3/cmake/using_flags.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/.codespell-ignore-lines` & `pyrf24-0.2.3/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/CMakeLists.txt` & `pyrf24-0.2.3/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/LICENSE` & `pyrf24-0.2.3/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/attr.h` & `pyrf24-0.2.3/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/buffer_info.h` & `pyrf24-0.2.3/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/cast.h` & `pyrf24-0.2.3/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/chrono.h` & `pyrf24-0.2.3/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/complex.h` & `pyrf24-0.2.3/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/detail/class.h` & `pyrf24-0.2.3/pybind11/include/pybind11/detail/class.h`

 * *Files 1% similar despite different names*

```diff
@@ -441,17 +441,25 @@
         clear_patients(self);
     }
 }
 
 /// Instance destructor function for all pybind11 types. It calls `type_info.dealloc`
 /// to destroy the C++ object itself, while the rest is Python bookkeeping.
 extern "C" inline void pybind11_object_dealloc(PyObject *self) {
+    auto *type = Py_TYPE(self);
+
+    // If this is a GC tracked object, untrack it first
+    // Note that the track call is implicitly done by the
+    // default tp_alloc, which we never override.
+    if (PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC) != 0) {
+        PyObject_GC_UnTrack(self);
+    }
+
     clear_instance(self);
 
-    auto *type = Py_TYPE(self);
     type->tp_free(self);
 
 #if PY_VERSION_HEX < 0x03080000
     // `type->tp_dealloc != pybind11_object_dealloc` means that we're being called
     // as part of a derived type's dealloc, in which case we're not allowed to decref
     // the type here. For cross-module compatibility, we shouldn't compare directly
     // with `pybind11_object_dealloc`, but with the common one stashed in internals.
```

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/detail/common.h` & `pyrf24-0.2.3/pybind11/include/pybind11/detail/common.h`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
 #define PYBIND11_VERSION_MINOR 10
-#define PYBIND11_VERSION_PATCH 3
+#define PYBIND11_VERSION_PATCH 4
 
 // Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
 // Additional convention: 0xD = dev
-#define PYBIND11_VERSION_HEX 0x020A0300
+#define PYBIND11_VERSION_HEX 0x020A0400
 
 // Define some generic pybind11 helper macros for warning management.
 //
 // Note that compiler-specific push/pop pairs are baked into the
 // PYBIND11_NAMESPACE_BEGIN/PYBIND11_NAMESPACE_END pair of macros. Therefore manual
 // PYBIND11_WARNING_PUSH/PYBIND11_WARNING_POP are usually only needed in `#include` sections.
 //
@@ -433,15 +433,15 @@
         }                                                                                         \
         PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
     }                                                                                             \
     PyObject *pybind11_init()
 
 /** \rst
     This macro creates the entry point that will be invoked when the Python interpreter
-    imports an extension module. The module name is given as the fist argument and it
+    imports an extension module. The module name is given as the first argument and it
     should not be in quotes. The second macro argument defines a variable of type
     `py::module_` which can be used to initialize the module.
 
     The entry point is marked as "maybe unused" to aid dead-code detection analysis:
     since the entry point is typically only looked up at runtime and not referenced
     during translation, it would otherwise appear as unused ("dead") code.
```

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/detail/descr.h` & `pyrf24-0.2.3/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/detail/init.h` & `pyrf24-0.2.3/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/detail/internals.h` & `pyrf24-0.2.3/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/detail/type_caster_base.h` & `pyrf24-0.2.3/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/detail/typeid.h` & `pyrf24-0.2.3/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/eigen/matrix.h` & `pyrf24-0.2.3/pybind11/include/pybind11/eigen/matrix.h`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,17 @@
    See also:
        https://stackoverflow.com/questions/2579576/i-dir-vs-isystem-dir
        https://stackoverflow.com/questions/1741816/isystem-for-ms-visual-studio-c-compiler
 */
 PYBIND11_WARNING_PUSH
 PYBIND11_WARNING_DISABLE_MSVC(5054) // https://github.com/pybind/pybind11/pull/3741
 //       C5054: operator '&': deprecated between enumerations of different types
+#if defined(__MINGW32__)
 PYBIND11_WARNING_DISABLE_GCC("-Wmaybe-uninitialized")
+#endif
 
 #include <Eigen/Core>
 #include <Eigen/SparseCore>
 
 PYBIND11_WARNING_POP
 
 // Eigen prior to 3.2.7 doesn't have proper move constructors--but worse, some classes get implicit
```

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/eigen/tensor.h` & `pyrf24-0.2.3/pybind11/include/pybind11/eigen/tensor.h`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 static_assert(__GNUC__ > 5, "Eigen Tensor support in pybind11 requires GCC > 5.0");
 #endif
 
 // Disable warnings for Eigen
 PYBIND11_WARNING_PUSH
 PYBIND11_WARNING_DISABLE_MSVC(4554)
 PYBIND11_WARNING_DISABLE_MSVC(4127)
+#if defined(__MINGW32__)
 PYBIND11_WARNING_DISABLE_GCC("-Wmaybe-uninitialized")
+#endif
 
 #include <unsupported/Eigen/CXX11/Tensor>
 
 PYBIND11_WARNING_POP
 
 static_assert(EIGEN_VERSION_AT_LEAST(3, 3, 0),
               "Eigen Tensor support in pybind11 requires Eigen >= 3.3.0");
```

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/embed.h` & `pyrf24-0.2.3/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/eval.h` & `pyrf24-0.2.3/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/functional.h` & `pyrf24-0.2.3/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/gil.h` & `pyrf24-0.2.3/pybind11/include/pybind11/gil.h`

 * *Files 2% similar despite different names*

```diff
@@ -148,16 +148,16 @@
             // Python >= 3.7 can remove this, it's an int before 3.7
             // NOLINTNEXTLINE(readability-qualified-auto)
             auto key = internals.tstate;
             PYBIND11_TLS_DELETE_VALUE(key);
         }
     }
 
-    gil_scoped_release(const gil_scoped_acquire &) = delete;
-    gil_scoped_release &operator=(const gil_scoped_acquire &) = delete;
+    gil_scoped_release(const gil_scoped_release &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
 
     /// This method will disable the PyThreadState_DeleteCurrent call and the
     /// GIL won't be acquired. This method should be used if the interpreter
     /// could be shutting down when this is called, as thread deletion is not
     /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
     /// protect subsequent code.
     PYBIND11_NOINLINE void disarm() { active = false; }
@@ -199,15 +199,15 @@
 
 class gil_scoped_release {
     PyThreadState *state;
 
 public:
     gil_scoped_release() : state{PyEval_SaveThread()} {}
     gil_scoped_release(const gil_scoped_release &) = delete;
-    gil_scoped_release &operator=(const gil_scoped_acquire &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     ~gil_scoped_release() { PyEval_RestoreThread(state); }
     void disarm() {}
 };
 
 #    endif // PYBIND11_SIMPLE_GIL_MANAGEMENT
 
 #else // WITH_THREAD
@@ -226,14 +226,14 @@
 class gil_scoped_release {
 public:
     gil_scoped_release() {
         // Trick to suppress `unused variable` error messages (at call sites).
         (void) (this != (this + 1));
     }
     gil_scoped_release(const gil_scoped_release &) = delete;
-    gil_scoped_release &operator=(const gil_scoped_acquire &) = delete;
+    gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     void disarm() {}
 };
 
 #endif // WITH_THREAD
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/iostream.h` & `pyrf24-0.2.3/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/numpy.h` & `pyrf24-0.2.3/pybind11/include/pybind11/numpy.h`

 * *Files 1% similar despite different names*

```diff
@@ -1117,18 +1117,18 @@
     template <ssize_t Dims = -1>
     detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
         return array::mutable_unchecked<T, Dims>();
     }
 
     /**
      * Returns a proxy object that provides const access to the array's data without bounds or
-     * dimensionality checking.  Unlike `unchecked()`, this does not require that the underlying
-     * array have the `writable` flag.  Use with care: the array must not be destroyed or reshaped
-     * for the duration of the returned object, and the caller must take care not to access invalid
-     * dimensions or dimension indices.
+     * dimensionality checking.  Unlike `mutable_unchecked()`, this does not require that the
+     * underlying array have the `writable` flag.  Use with care: the array must not be destroyed
+     * or reshaped for the duration of the returned object, and the caller must take care not to
+     * access invalid dimensions or dimension indices.
      */
     template <ssize_t Dims = -1>
     detail::unchecked_reference<T, Dims> unchecked() const & {
         return array::unchecked<T, Dims>();
     }
 
     /// Ensure that the argument is a NumPy array of the correct dtype (and if not, try to convert
```

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/operators.h` & `pyrf24-0.2.3/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/options.h` & `pyrf24-0.2.3/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/pybind11.h` & `pyrf24-0.2.3/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/pytypes.h` & `pyrf24-0.2.3/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/stl/filesystem.h` & `pyrf24-0.2.3/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/stl.h` & `pyrf24-0.2.3/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/include/pybind11/stl_bind.h` & `pyrf24-0.2.3/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/noxfile.py` & `pyrf24-0.2.3/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/pybind11/__main__.py` & `pyrf24-0.2.3/pybind11/pybind11/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=missing-function-docstring
 
 import argparse
 import sys
 import sysconfig
 
+from ._version import __version__
 from .commands import get_cmake_dir, get_include, get_pkgconfig_dir
 
 
 def print_includes() -> None:
     dirs = [
         sysconfig.get_path("include"),
         sysconfig.get_path("platinclude"),
@@ -20,17 +21,22 @@
         if d and d not in unique_dirs:
             unique_dirs.append(d)
 
     print(" ".join("-I" + d for d in unique_dirs))
 
 
 def main() -> None:
-
     parser = argparse.ArgumentParser()
     parser.add_argument(
+        "--version",
+        action="version",
+        version=__version__,
+        help="Print the version and exit.",
+    )
+    parser.add_argument(
         "--includes",
         action="store_true",
         help="Include flags for both pybind11 and Python headers.",
     )
     parser.add_argument(
         "--cmakedir",
         action="store_true",
```

### Comparing `pyrf24-0.2.2/pybind11/pybind11/commands.py` & `pyrf24-0.2.3/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/pybind11/setup_helpers.py` & `pyrf24-0.2.3/pybind11/pybind11/setup_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     def _add_cflags(self, flags: List[str]) -> None:
         self.extra_compile_args[:0] = flags
 
     def _add_ldflags(self, flags: List[str]) -> None:
         self.extra_link_args[:0] = flags
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-
         self._cxx_level = 0
         cxx_std = kwargs.pop("cxx_std", 0)
 
         if "language" not in kwargs:
             kwargs["language"] = "c++"
 
         include_pybind11 = kwargs.pop("include_pybind11", True)
@@ -170,17 +169,18 @@
         add a macos-min 10.9 or 10.14 flag if MACOSX_DEPLOYMENT_TARGET is
         unset.
         """
         return self._cxx_level
 
     @cxx_std.setter
     def cxx_std(self, level: int) -> None:
-
         if self._cxx_level:
-            warnings.warn("You cannot safely change the cxx_level after setting it!")
+            warnings.warn(
+                "You cannot safely change the cxx_level after setting it!", stacklevel=2
+            )
 
         # MSVC 2015 Update 3 and later only have 14 (and later 17) modes, so
         # force a valid flag here.
         if WIN and level == 11:
             level = 14
 
         self._cxx_level = level
@@ -435,15 +435,14 @@
             macros: Optional[Union[Tuple[str], Tuple[str, Optional[str]]]] = None,
             include_dirs: Optional[List[str]] = None,
             debug: bool = False,
             extra_preargs: Optional[List[str]] = None,
             extra_postargs: Optional[List[str]] = None,
             depends: Optional[List[str]] = None,
         ) -> Any:
-
             # These lines are directly from distutils.ccompiler.CCompiler
             macros, objects, extra_postargs, pp_opts, build = compiler._setup_compile(  # type: ignore[attr-defined]
                 output_dir, macros, include_dirs, sources, depends, extra_postargs
             )
             cc_args = compiler._get_cc_args(pp_opts, debug, extra_preargs)  # type: ignore[attr-defined]
 
             # The number of threads; start with default.
```

### Comparing `pyrf24-0.2.2/pybind11/pyproject.toml` & `pyrf24-0.2.3/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/setup.cfg` & `pyrf24-0.2.3/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/setup.py` & `pyrf24-0.2.3/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/FindCatch.cmake` & `pyrf24-0.2.3/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/FindEigen3.cmake` & `pyrf24-0.2.3/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/FindPythonLibsNew.cmake` & `pyrf24-0.2.3/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/JoinPaths.cmake` & `pyrf24-0.2.3/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/check-style.sh` & `pyrf24-0.2.3/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/cmake_uninstall.cmake.in` & `pyrf24-0.2.3/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pyrf24-0.2.3/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/libsize.py` & `pyrf24-0.2.3/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/make_changelog.py` & `pyrf24-0.2.3/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/pybind11Common.cmake` & `pyrf24-0.2.3/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/pybind11Config.cmake.in` & `pyrf24-0.2.3/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/pybind11NewTools.cmake` & `pyrf24-0.2.3/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/pybind11Tools.cmake` & `pyrf24-0.2.3/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/setup_global.py.in` & `pyrf24-0.2.3/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pybind11/tools/setup_main.py.in` & `pyrf24-0.2.3/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pyproject.toml` & `pyrf24-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/pyrf24.egg-info/PKG-INFO` & `pyrf24-0.2.3/pyrf24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrf24
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python package for the wrapping nRF24 related C++ libraries.
 Author-email: Brendan Doherty <2bndy5@gmail.com>
 License: GPLv2
 Project-URL: Documentation, http://nRF24.github.io/pyRF24
 Project-URL: Source, https://github.com/nRF24/pyRF24
 Project-URL: Tracker, https://github.com/nRF24/pyRF24/issues
 Keywords: nrf24l01,nRF24L01+,raspberry,pi,driver,radio,transceiver
```

### Comparing `pyrf24-0.2.2/pyrf24.egg-info/SOURCES.txt` & `pyrf24-0.2.3/pyrf24.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/setup.py` & `pyrf24-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyRF24.cpp` & `pyrf24-0.2.3/src/pyRF24.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyRF24Mesh.cpp` & `pyrf24-0.2.3/src/pyRF24Mesh.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyRF24Network.cpp` & `pyrf24-0.2.3/src/pyRF24Network.cpp`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyrf24/__init__.py` & `pyrf24-0.2.3/src/pyrf24/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyrf24/fake_ble.py` & `pyrf24-0.2.3/src/pyrf24/fake_ble.py`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyrf24/rf24.pyi` & `pyrf24-0.2.3/src/pyrf24/rf24.pyi`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyrf24/rf24_mesh.pyi` & `pyrf24-0.2.3/src/pyrf24/rf24_mesh.pyi`

 * *Files identical despite different names*

### Comparing `pyrf24-0.2.2/src/pyrf24/rf24_network.pyi` & `pyrf24-0.2.3/src/pyrf24/rf24_network.pyi`

 * *Files identical despite different names*

