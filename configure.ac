AC_PREREQ(2.52)

AC_INIT([Apertium Romanian], [1.0.0], [apertium-stuff@lists.sourceforge.net], [apertium-ron], [https://wiki.apertium.org/wiki/Apertium-ron])
AM_INIT_AUTOMAKE

PKG_CHECK_MODULES(APERTIUM, apertium >= 3.6.0)
PKG_CHECK_MODULES(LTTOOLBOX, lttoolbox >= 3.5.0)
PKG_CHECK_MODULES(CG3, cg3 >= 1.3.0)

PKG_CHECK_MODULES(REGTEST, apertium-regtest >= 0.0.1, [],
                  [AC_MSG_WARN([Running tests requires apertium-regtest])])

AP_MKINCLUDE

AC_OUTPUT([Makefile apertium-ron.pc])
