SUBDIR=		bootstrap \
		dataTables
NO_OBJ=		yes
PREFIX?=	/usr/local
FILESDIR=	${PREFIX}/share/poudriere/html/assets
FILES=		jquery-1.9.1.min.js \
		logo.jpg \
		poudriere.css \
		poudriere.js

beforeinstall:
	mkdir -p ${DESTDIR}${FILESDIR}

.include <bsd.prog.mk>
