#	$NetBSD: Makefile,v 1.11 2020/04/13 11:27:22 jdolecek Exp $
#

.PATH:	${.CURDIR}/../../../../dev/usb

LIB=	rumpdev_umass
COMMENT=USB mass storage driver

IOCONF=	UMASS.ioconf

.if ${MACHINE} == "i386" || ${MACHINE} == "amd64"
SRCS=	umass.c umass_quirks.c umass_scsipi.c

SRCS+=	umass_component.c
.else
SRCS=	dummy.c
.endif

.include <bsd.lib.mk>
.include <bsd.klinks.mk>
