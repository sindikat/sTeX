# recurse into the directories. 
DISTDIRS = core 
MAKEDIRS = $(DISTDIRS) obsolete experiments

all package doc clean distclean stycls: 
	@for d in $(MAKEDIRS); do (cd $$d && $(MAKE) -$(MAKEFLAGS) $@) || exit $$?; done

ltds lctan filedate checksum enablechecksum disablechecksum: 
	@for d in $(DISTDIRS); do (cd $$d && $(MAKE) -$(MAKEFLAGS) $@) || exit $$?; done


