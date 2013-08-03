TESTS = run-test.sh
TESTS_ENVIRONMENT = NO_MAKE=yes CUTTER="$(CUTTER)"

noinst_LTLIBRARIES = test_stack.la

INCLUDES = $(CPPCUTTER_CFLAGS) -l$(top_srcdir)/src
LIBS = $(CPPCUTTER_LIBS) $(top_builddir)/src/libstack.la

LDFLAGS = -module -rpath $(libdir) -avoid-version -no-undefined

test_stack_la_SOURCES = test-stack.cpp

echo-cutter:
	@echo	$(CUTTER)
