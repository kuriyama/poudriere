# $DragonFly: src/bin/cpdup/Makefile,v 1.7 2008/04/10 22:09:08 dillon Exp $
#

PREFIX?=	/usr/local
BINDIR=		${PREFIX}/libexec/poudriere

PROG=	cpdup
SRCS=	cpdup.c hcproto.c hclink.c misc.c fsmid.c

NO_MAN=	yes

.if defined(.FreeBSD)
CFLAGS += -D_ST_FLAGS_PRESENT_=1
WARNS?=	6
.endif

.if !defined(NOMD5)
SRCS+=	md5.c
.endif

LDADD+= -lmd
DPADD+= ${LIBMD}

.include <bsd.prog.mk>

