NAME=percolate
CSYM=percolate

current: pd_nt pd_linux pd_darwin

# ----------------------- NT -----------------------

pd_nt: $(NAME).dll

.SUFFIXES: .dll

PDNTCFLAGS = /W3 /WX /DNT /DPD /nologo
VC="C:\Programme\Microsoft Visual Studio\VC98"

PDNTINCLUDE = /I. /Ic:\pd\tcl\include /Ic:\pd\src /I$(VC)\include /I_headers /I_source

PDNTLDIR = $(VC)\Lib
PDNTLIB = $(PDNTLDIR)\libc.lib \
	$(PDNTLDIR)\oldnames.lib \
	$(PDNTLDIR)\kernel32.lib \
	$(PDNTLDIR)\user32.lib \
	$(PDNTLDIR)\uuid.lib \
	c:\pd\bin\pd.lib

EXTERNALS = flute~.obj mandolin~.obj plucked~.obj bowed~.obj bowedbar~.obj \
            clar~.obj brass~.obj blotar~.obj marimba~.obj vibraphone~.obj \
            agogo~.obj bamboo~.obj cabasa~.obj sleigh~.obj guiro~.obj \
            chase~.obj escalator~.obj jitter~.obj klutz~.obj random~.obj \
            flip~.obj weave~.obj dcblock~.obj gQ~.obj munger~.obj scrub~.obj \
            absmin~.obj absmax~.obj terrain~.obj gen5.obj gen7.obj gen9.obj \
            gen10.obj gen17.obj gen24.obj gen25.obj metashake~.obj waffle~.obj \
            sekere~.obj shaker~.obj tamb~.obj wuter~.obj

.c.dll:
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "_source\stk.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\blotar\blotar~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\bowed\bowed~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\bowed bar\bowedbar~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\brass\brass~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\clarinet\clar~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\flute\flute~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\mandolin\mandolin~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "1. Physical Models\plucked\plucked~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "2. Modal Synthesis\agogo\agogo~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "2. Modal Synthesis\marimba\marimba~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "2. Modal Synthesis\vibraphone\vibraphone~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\bamboo\bamboo~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\cabasa\cabasa~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\guiro\guiro~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\meta-shaker\metashake~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\sekere\sekere~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\shaker\shaker~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\sleigh bells\sleigh~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\tamb\tamb~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "3. PhISM\wuter\wuter~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen10\gen10.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen17\gen17.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen20\gen20.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen24\gen24.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen25\gen25.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen5\gen5.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen7\gen7.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "4. MaxGens\gen9\gen9.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\absmax~\absmax~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\absmin~\absmin~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\chase~\chase~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\escal~\escalator~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\flip~\flip~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\jitter~\jitter~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\klutz~\klutz~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\random~\random~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\terrain~\terrain~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\waffle~\waffle~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "5. SID\weave~\weave~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "6. Random DSP\dcblock\dcblock~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "6. Random DSP\gQ\gQ~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "6. Random DSP\munger\munger~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "6. Random DSP\scrubber\scrub~.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c "_source\stk.c"
	cl $(PDNTCFLAGS) $(PDNTINCLUDE) /c $*.c
	link /dll /out:../PeRColate.dll /export:$(CSYM)_setup $*.obj stk.obj $(EXTERNALS) $(PDNTLIB)

# ----------------------- LINUX i386 -----------------------

pd_linux: $(NAME).pd_linux

.SUFFIXES: .pd_linux

PATH1=1.\ Physical\ Models
PATH2=2.\ Modal\ Synthesis
PATH3=3.\ PhISM
PATH4=4.\ MaxGens
PATH5=5.\ SID
PATH6=6.\ Random\ DSP

LINUX_SOURCES = percolate.c				\
		 _source/stk.c				\
		$(PATH1)/blotar/blotar~.c		\
		$(PATH1)/bowed/bowed~.c			\
		$(PATH1)/bowed\ bar/bowedbar~.c		\
		$(PATH1)/brass/brass~.c			\
		$(PATH1)/clarinet/clar~.c		\
		$(PATH1)/flute/flute~.c			\
		$(PATH1)/mandolin/mandolin~.c		\
		$(PATH1)/plucked/plucked~.c		\
		$(PATH2)/agogo/agogo~.c			\
		$(PATH2)/marimba/marimba~.c		\
		$(PATH2)/vibraphone/vibraphone~.c	\
		$(PATH3)/bamboo/bamboo~.c		\
		$(PATH3)/cabasa/cabasa~.c		\
		$(PATH3)/meta-shaker/metashake~.c	\
		$(PATH3)/sekere/sekere~.c		\
		$(PATH3)/sleigh\ bells/sleigh~.c	\
		$(PATH3)/shaker/shaker~.c		\
		$(PATH3)/guiro/guiro~.c			\
		$(PATH3)/tamb/tamb~.c			\
		$(PATH3)/wuter/wuter~.c			\
		$(PATH4)/gen10/gen10.c			\
		$(PATH4)/gen17/gen17.c			\
		$(PATH4)/gen20/gen20.c			\
		$(PATH4)/gen24/gen24.c			\
		$(PATH4)/gen25/gen25.c			\
		$(PATH4)/gen5/gen5.c			\
		$(PATH4)/gen7/gen7.c			\
		$(PATH4)/gen9/gen9.c			\
		$(PATH5)/absmax~/absmax~.c		\
		$(PATH5)/absmin~/absmin~.c		\
		$(PATH5)/chase~/chase~.c		\
		$(PATH5)/escal~/escalator~.c		\
		$(PATH5)/flip~/flip~.c			\
		$(PATH5)/jitter~/jitter~.c		\
		$(PATH5)/klutz~/klutz~.c		\
		$(PATH5)/random~/random~.c		\
		$(PATH5)/terrain~/terrain~.c		\
		$(PATH5)/waffle~/waffle~.c		\
		$(PATH5)/weave~/weave~.c		\
		$(PATH6)/dcblock/dcblock~.c		\
		$(PATH6)/gQ/gQ~.c			\
		$(PATH6)/munger/munger~.c		\
		$(PATH6)/scrubber/scrub~.c

LINUX_OBJECTS = $(LINUX_SOURCES:.c=.o)

LINUX_OBJECTS2 = percolate.o				\
		_source/stk.o				\
		$(PATH1)/blotar/blotar~.o		\
		$(PATH1)/bowed/bowed~.o		\
		$(PATH1)/bowed\ bar/bowedbar~.o	\
		$(PATH1)/brass/brass~.o		\
		$(PATH1)/clarinet/clar~.o		\
		$(PATH1)/flute/flute~.o		\
		$(PATH1)/mandolin/mandolin~.o		\
		$(PATH1)/plucked/plucked~.o		\
		$(PATH2)/agogo/agogo~.o		\
		$(PATH2)/marimba/marimba~.o		\
		$(PATH2)/vibraphone/vibraphone~.o	\
		$(PATH3)/bamboo/bamboo~.o		\
		$(PATH3)/cabasa/cabasa~.o		\
		$(PATH3)/meta-shaker/metashake~.o	\
		$(PATH3)/sekere/sekere~.o		\
		$(PATH3)/shaker/shaker~.o		\
		$(PATH3)/guiro/guiro~.o		\
		$(PATH3)/sleigh\ bells/sleigh~.o	\
		$(PATH3)/tamb/tamb~.o			\
		$(PATH3)/wuter/wuter~.o		\
		$(PATH4)/gen10/gen10.o		\
		$(PATH4)/gen17/gen17.o		\
		$(PATH4)/gen20/gen20.o		\
		$(PATH4)/gen24/gen24.o		\
		$(PATH4)/gen25/gen25.o		\
		$(PATH4)/gen5/gen5.o			\
		$(PATH4)/gen7/gen7.o			\
		$(PATH4)/gen9/gen9.o			\
		$(PATH5)/absmax~/absmax~.o		\
		$(PATH5)/absmin~/absmin~.o		\
		$(PATH5)/chase~/chase~.o		\
		$(PATH5)/escal~/escalator~.o		\
		$(PATH5)/flip~/flip~.o			\
		$(PATH5)/jitter~/jitter~.o		\
		$(PATH5)/klutz~/klutz~.o		\
		$(PATH5)/random~/random~.o		\
		$(PATH5)/terrain~/terrain~.o		\
		$(PATH5)/waffle~/waffle~.o		\
		$(PATH5)/weave~/weave~.o		\
		$(PATH6)/dcblock/dcblock~.o		\
		$(PATH6)/gQ/gQ~.o			\
		$(PATH6)/munger/munger~.o		\
		$(PATH6)/scrubber/scrub~.o


LINUXCFLAGS = -DPD -DUNIX -DICECAST -O2 -funroll-loops -fomit-frame-pointer \
    -Wall -W -Wshadow -Wstrict-prototypes -Werror \
    -Wno-unused -Wno-parentheses -Wno-switch

LINUXINCLUDE =  -I _headers -I ../../pd/pd-0.36-test5/src/

.c.o:
	cc $(LINUXCFLAGS) $(LINUXINCLUDE) -o "$*.o" -c "$*.c"

$(NAME).pd_linux: $(LINUX_OBJECTS)
	ld -export_dynamic  -shared -o $*.pd_linux $(LINUX_OBJECTS2) -lc -lm
	strip --strip-unneeded $*.pd_linux
	rm -f $*.o ../$*.pd_linux
	ln -s $*/$*.pd_linux ..

clean_linux:
	find -name "*.o" -exec rm \{\} \;
	rm *.pd_*

# ----------------------- MAC OS X -----------------------

pd_darwin: $(NAME).pd_darwin

.SUFFIXES: .pd_darwin .pd_darwin_o


MACOSXCFLAGS = -DPD -DUNIX -DMACOSX -O3 \
    -Wall -W -Wstrict-prototypes \
    -Wno-unused -Wno-parentheses -Wno-switch

PD = ../../pd/bin/pd

MACOSXLDFLAGS = -bundle -bundle_loader $(PD) -flat_namespace

MACOSXINCLUDE =  -I _headers -I ../../pd/src/

MACOSX_OBJECTS = $(LINUX_SOURCES:.c=.pd_darwin_o)
MACOSX_OBJECTS2 = $(LINUX_OBJECTS2:.o=.pd_darwin_o)

.c.pd_darwin_o:
	cc $(MACOSXCFLAGS) $(MACOSXINCLUDE) -o "$*.pd_darwin_o" -c "$*.c"

$(NAME).pd_darwin: $(MACOSX_OBJECTS)
	cc $(MACOSXLDFLAGS) -o $*.pd_darwin $(MACOSX_OBJECTS2) -lc -lm
	rm -f $*.o ../$*.pd_darwin
	ln -s $*/$*.pd_darwin ..

clean_darwin:
	find . -name "*.pd_darwin_o" -exec rm \{\} \;
	rm *.pd_*

