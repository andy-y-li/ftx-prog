#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT(ftx-prog, 1.0, [andy_y_li@163.com])
AM_INIT_AUTOMAKE
AC_CONFIG_SRCDIR([src/ftx_prog.c])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CC

# Checks for libraries.
# FIXME: Replace `main' with a function in `-lftdi':
AC_CHECK_LIB([ftdi], [main])
# FIXME: Replace `main' with a function in `-lusb':
AC_CHECK_LIB([usb], [main])

# Checks for header files.
AC_CHECK_HEADERS([fcntl.h stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL

# Checks for library functions.
AC_FUNC_MALLOC
AC_CHECK_FUNCS([atexit memset strcasecmp strrchr strtoul])

#AC_CONFIG_FILES([Makefile])
AC_OUTPUT([Makefile])
