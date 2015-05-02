VIDEOS=RMS-W3-D1.ogv RMS-W3-D2.ogv

RM=rm -f
WGET=wget
URL_ROOT=http://vrepin.org/rms/W3/


all: $(VIDEOS)

RMS-W3-D1.ogv:
	$(WGET) $(URL_ROOT)$@

RMS-W3-D2.ogv:
	$(WGET) $(URL_ROOT)$@


clean:
	$(RM) $(VIDEOS)
