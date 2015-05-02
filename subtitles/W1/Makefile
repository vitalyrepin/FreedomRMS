VIDEOS= RMS-W1_V1.ogv RMS-W1_V2.ogv RMS-W1_V3.ogv
RM=rm -f
WGET=wget
URL_ROOT=http://vrepin.org/rms/W1/

all: $(VIDEOS)

RMS-W1_V1.ogv:
	$(WGET) $(URL_ROOT)$@

RMS-W1_V2.ogv:
	$(WGET) $(URL_ROOT)$@

RMS-W1_V3.ogv:
	$(WGET) $(URL_ROOT)$@

clean:
	$(RM) $(VIDEOS)
