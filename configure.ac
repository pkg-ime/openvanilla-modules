#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.63])
AC_INIT([openvanilla-modules], [0.9.0a1.3], [])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])
AC_CONFIG_SRCDIR([configure.ac])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_MAKE_SET
AC_PROG_LIBTOOL

# Checks for libraries.
AC_CHECK_LIB([sqlite3], [main])


# Checks for header files.
AC_HEADER_DIRENT
AC_HEADER_STDC
AC_CHECK_HEADERS([fcntl.h stdlib.h string.h sys/param.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_HEADER_STDBOOL
AC_C_CONST
AC_C_INLINE
AC_TYPE_SIZE_T
AC_STRUCT_TM

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_MEMCMP
AC_FUNC_MMAP
AC_FUNC_SELECT_ARGTYPES
AC_FUNC_STAT
AC_FUNC_REALLOC
AC_CHECK_FUNCS([bzero mkdir munmap rmdir select strcasecmp strchr strcspn strspn strstr strtol])

# data tables options

AC_ARG_ENABLE([asia],
            [AS_HELP_STRING([--enable-asia],
              [enable input methods collection for asia common (default=yes)])],
            [with__asia="$enableval"],
            [with__asia=yes])
AM_CONDITIONAL(WITH_asia, test x$with__asia != xno )

AC_ARG_ENABLE([th_TH],
            [AS_HELP_STRING([--enable-th_TH],
              [enable input methods collection for th_TH])],
            [with_th_TH=yes],
            [with_th_TH=no])
AM_CONDITIONAL(WITH_th_TH, test x$with_th_TH != xno )

AC_ARG_ENABLE([vi_VN],
            [AS_HELP_STRING([--enable-vi_VN],
              [enable input methods collection for vi_VN])],
            [with_vi_VN=yes],
            [with_vi_VN=no])
AM_CONDITIONAL(WITH_vi_VN, test x$with_vi_VN != xno )

AC_ARG_ENABLE([jp_JP],
            [AS_HELP_STRING([--enable-jp_JP],
              [enable input methods collection for jp_JP])],
            [with_jp_JP=yes],
            [with_jp_JP=no])
AM_CONDITIONAL(WITH_jp_JP, test x$with_jp_JP != xno )

AC_ARG_ENABLE([ko_KR],
            [AS_HELP_STRING([--enable-ko_KR],
              [enable input methods collection for ko_KR])],
            [with_ko_KR=yes],
            [with_ko_KR=no])
AM_CONDITIONAL(WITH_ko_KR, test x$with_ko_KR != xno )

AC_ARG_ENABLE([zh_CN],
            [AS_HELP_STRING([--enable-zh_CN],
              [enable input methods collection for zh_CN])],
            [with_zh_CN=yes],
            [with_zh_CN=no])
AM_CONDITIONAL(WITH_zh_CN, test x$with_zh_CN != xno )

AC_ARG_ENABLE([zh_HK],
            [AS_HELP_STRING([--enable-zh_HK],
              [enable input methods collection for zh_HK])],
            [with_zh_HK=yes],
            [with_zh_HK=no])
AM_CONDITIONAL(WITH_zh_HK, test x$with_zh_HK != xno )

AC_ARG_ENABLE([zh_TW],
            [AS_HELP_STRING([--enable-zh_TW],
              [enable input methods collection for zh_TW])],
            [with_zh_TW=yes],
            [with_zh_TW=no])
AM_CONDITIONAL(WITH_zh_TW, test x$with_zh_TW != xno )

AC_ARG_ENABLE([zh_TW_hakka],
            [AS_HELP_STRING([--enable-zh_TW_hakka],
              [enable input methods collection for zh_TW hakka])],
            [with_zh_TW_hakka=yes],
            [with_zh_TW_hakka=no])
AM_CONDITIONAL(WITH_zh_TW_hakka, test x$with_zh_TW_hakka != xno )

AC_ARG_ENABLE([zh_TW_taigi],
            [AS_HELP_STRING([--enable-zh_TW_taigi],
              [enable input methods collection for zh_TW taigi])],
            [with_zh_TW_taigi=yes],
            [with_zh_TW_taigi=no])
AM_CONDITIONAL(WITH_zh_TW_taigi, test x$with_zh_TW_taigi != xno )


AC_MSG_RESULT([
Enabled input methods collections:
  asia          $with__asia
  ja            $with_jp_JP
  kr            $with_ko_KR
  th            $with_th_TH
  vi            $with_vi_VN
  zh_CN         $with_zh_CN
  zh_HK         $with_zh_HK
  zh_TW         $with_zh_TW
  zh_TW_hakka   $with_zh_TW_hakka
  zh_TW_taigi   $with_zh_TW_taigi
])



AC_CONFIG_FILES([
DataTables/Makefile
Frameworks/Makefile
Frameworks/OpenVanilla/Headers/Makefile
Frameworks/OpenVanilla/Makefile
Frameworks/OpenVanilla/Source/Makefile
Makefile
Modules/Makefile
Modules/OVIMGeneric/Makefile
Modules/SharedLibrary/Makefile
])


AC_OUTPUT
