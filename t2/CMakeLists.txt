CMAKE_MINIMUM_REQUIRED(VERSION 3.16)
PROJECT(HELLO)
INSTALL(FILES COPYRIGHT README DESTINATION share/doc/cmake/t2)
INSTALL(PROGRAMS runhello.sh DESTINATION bin)
ADD_SUBDIRECTORY(src bin)




