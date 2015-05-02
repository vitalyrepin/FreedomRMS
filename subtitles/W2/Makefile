VIDEOS= RMS-W2-D1.ogv RMS-W2-D2.ogv RMS-W2-D3.ogv RMS-W2-D4.webm
RM=rm -f
WGET=wget
URL_ROOT=http://vrepin.org/rms/W2/

all: $(VIDEOS)

RMS-W2-D1.ogv:
	$(WGET) $(URL_ROOT)$@

RMS-W2-D2.ogv:
	$(WGET) $(URL_ROOT)$@

RMS-W2-D3.ogv:
	$(WGET) $(URL_ROOT)$@

RMS-W2-D4.webm:
	$(WGET) $(URL_ROOT)$@

clean:
	$(RM) $(VIDEOS)
