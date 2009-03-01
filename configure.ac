AC_PREREQ(2.61)
AC_INIT([NULLants],[0.0.1],[m3lawren@uwaterloo.ca])
AM_INIT_AUTOMAKE([])
AC_CONFIG_MACRO_DIR([m4])

# Tools 
AC_PROG_CC
AC_PROG_CXX

# Functions

# Language features

# Arguments
AC_ARG_ENABLE(
	[coverage],
	AS_HELP_STRING([--enable-coverage],[Enables coverage checking. This clobbers CFLAGS and CXXFLAGS.]),
	[AC_SUBST(
		[CFLAGS],
		["-ftest-coverage -fprofile-arcs -g"])
	 AC_SUBST(
	 	[CXXFLAGS],
		["-ftest-coverage -fprofile-arcs -g"])],
	[])

AC_CONFIG_HEADER([config.h])
AC_CONFIG_FILES([
	Makefile
	src/Makefile
])

AC_OUTPUT
