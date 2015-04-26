VIDEOS= RMS-W2-D1.ogv RMS-W2-D2.ogv RMS-W2-D3.ogv RMS-W2-D4.webm
RM=rm -f
WGET=wget

all: $(VIDEOS)

RMS-W2-D1.ogv:
	$(WGET) http://vrepin.org/rms/W2/RMS-W2-D1.ogv

RMS-W2-D2.ogv:
	$(WGET) http://vrepin.org/rms/W2/RMS-W2-D2.ogv

RMS-W2-D3.ogv:
	$(WGET) http://vrepin.org/rms/W2/RMS-W2-D3.ogv

RMS-W2-D4.webm:
	$(WGET) http://vrepin.org/rms/W2/RMS-W2-D4.webm

clean:
	$(RM) $(VIDEOS)
