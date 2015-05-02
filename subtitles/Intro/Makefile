VIDEOS=IntroRMS.ogv
RM=rm -f
WGET=wget
URL_ROOT=http://vrepin.org/rms/Intro/

all: $(VIDEOS)

IntroRMS.ogv:
	$(WGET) $(URL_ROOT)$@

clean:
	$(RM) $(VIDEOS)
