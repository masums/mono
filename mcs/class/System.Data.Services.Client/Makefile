thisdir = class/System.Data.Services.Client
SUBDIRS = 
include ../../build/rules.make

LIBRARY = System.Data.Services.Client.dll

Client/System.Data.Services.Client.resources: Client/System.Data.Services.Client.txt
	$(RESGEN) "$<" "$@"

LIB_REFS = System System.Core System.Xml.Linq System.Data System.Xml
LIB_MCS_FLAGS = \
	-d:NET_3_5	\
	-r:System.dll \
	-r:System.Core.dll \
	-r:System.Xml.Linq.dll \
	-r:System.Data.dll \
	-r:System.Xml.dll \
	-resource:Client/System.Data.Services.Client.resources \
	-warn:2

ifneq (2.1, $(FRAMEWORK_VERSION))
LIB_REFS += WindowsBase
LIB_MCS_FLAGS += -r:WindowsBase
endif

include ../../build/library.make

$(the_lib): Client/System.Data.Services.Client.resources

EXTRA_DISTFILES = Client/System.Data.Services.Client.txt
CLEAN_FILES += Client/System.Data.Services.Client.resources
