####### This is the input file for automake, which will generate Makefile.in ##########
## not a GNU package. You can remove this line, if
## you have all needed files, that a GNU package needs
AUTOMAKE_OPTIONS = foreign 1.4

noinst_PROGRAMS = wstdemo
SOAPHEADER = wstdemo.h

include ../Makefile.defines
include ../Makefile.c_rules
SOAP_NS = wstdemo.nsmap

wstdemo_CFLAGS = -DWITH_DOM -DWITH_OPENSSL -DWITH_GZIP -DSKIP_CERTIFICATE_VERIFICATION
wstdemo_SOURCES = wstdemo.c $(SOAPHEADER) $(SOAP_C_SRC) ../../stdsoap2.c ../../dom.c ../../plugin/wstapi.c ../../plugin/wsseapi.c ../../plugin/wsaapi.c ../../plugin/smdevp.c ../../plugin/mecevp.c
wstdemo_LDADD = $(SAMPLE_EXTRA_LIBS) -lssl -lcrypto -lz
