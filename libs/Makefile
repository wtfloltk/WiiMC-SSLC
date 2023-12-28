COMMAND1 = (CC=$(DEVKITPPC)/bin/powerpc-eabi-gcc CXX=$(DEVKITPPC)/bin/powerpc-eabi-g++ ./configure --host=powerpc-eabi --build=powerpc-eabi-gnu --prefix="${DEVKITPRO}/portlibs/ppc" --libdir="${DEVKITPRO}/portlibs/ppc/lib" --disable-shared && \
      make && sudo -E make install)

all: dir1 dir2 dir3

dir1:
	cd fribidi && chmod +x configure && $(COMMAND1)
dir2:
	cd libexif && chmod +x configure && $(COMMAND1)
dir3:
	cd libiconv && chmod +x configure && $(COMMAND1)
