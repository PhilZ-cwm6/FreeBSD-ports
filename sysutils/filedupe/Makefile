PORTNAME=	filedupe
PORTVERSION=	1.1
PORTREVISION=	4
CATEGORIES=	sysutils
MASTER_SITES=	http://sammy.net/~sammy/hacks/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Utility for quickly finding duplicate files

LIB_DEPENDS=	libgdbm.so:databases/gdbm

PLIST_FILES=	bin/filedupe

post-patch:
	${REINPLACE_CMD} -e 's|filename\[80\]|filename[1024]|g; \
		s|your_database|/var/db/filedupe.db|' ${WRKSRC}/filedupe.c

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/filedupe ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
