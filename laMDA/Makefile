-include ~/.zdeck

ZDECK_HOME ?= /usr/share/zdeck
ZDECK_CLASS = lecture

images_dia = $(wildcard figures/*.dia)
images_png = $(images_dia:.dia=.png)

all: lamda.html

slides.html: $(images_png) $(datauris)

clean:
	rm -f $(images_png)
	rm -f lamda.html

include $(ZDECK_HOME)/stylesheets/Makefile.rules
