# $NetBSD: Makefile,v 1.2 2019/02/17 04:05:52 rin Exp $

.include "../Makefile.inc"

.PATH:  ${S}/net

KMOD=		if_stf
IOCONF=		stf.ioconf
SRCS=		if_stf.c

CPPFLAGS+=	-DINET
CPPFLAGS+=	-DINET6

WARNS=		3

.include <bsd.kmodule.mk>
