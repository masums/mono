thisdir = class/System.Net.Http
SUBDIRS = 
include ../../build/rules.make

LIBRARY = System.Net.Http.dll

LIB_REFS = System.Core System
LIB_MCS_FLAGS = -r:System.Core.dll -r:System.dll $(EXTRA_LIB_MCS_FLAGS)

TEST_MCS_FLAGS = -r:System.dll -r:System.Core.dll

include ../../build/library.make
