SOURCE = http://pyyaml.org/download/libyaml/yaml-0.1.7.tar.gz
TARGET = yaml-0.1.7.tar.gz
DIRECTORY = yaml-0.1.7

FETCH = wget

all: extract
	$(MAKE) -C $(DIRECTORY)

extract: $(DIRECTORY)
	cd $(DIRECTORY) ;\
	./configure

$(DIRECTORY): $(TARGET)
	tar zxf $(TARGET)

$(TARGET):
	$(FETCH) $(FETCH_OPT) $(SOURCE)

clean:
	$(RM) -R $(DIRECTORY) $(TARGET)

.PHONY: all clean
