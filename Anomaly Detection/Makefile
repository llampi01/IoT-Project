CONTIKI_PROJECT = DelayServer DelayClient packetLossServer unusualTraffic
all: $(CONTIKI_PROJECT)
CONTIKI = ../..

# The BR is either native or embedded, and in the latter case must support SLIP
PLATFORMS_EXCLUDE = z1

# Include RPL BR module
include $(CONTIKI)/Makefile.dir-variables
MODULES += $(CONTIKI_NG_SERVICES_DIR)/project
# Include webserver module
MODULES_REL += webserver
include $(CONTIKI)/Makefile.identify-target
MODULES += $(TARGET)
include $(CONTIKI)/Makefile.include
