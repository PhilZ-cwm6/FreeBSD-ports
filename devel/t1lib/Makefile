PORTNAME=	t1lib
PORTVERSION=	5.1.2
PORTREVISION=	5
PORTEPOCH=	1
CATEGORIES=	devel
MASTER_SITES=	SUNSITE/libs/graphics/

MAINTAINER=	ler@FreeBSD.org
COMMENT=	Type 1 font rasterization library for Unix/X11

LICENSE=	LGPL20
LICENSE_FILE=	${WRKSRC}/LGPL

USES=		cpe gmake libtool
USE_LDCONFIG=	yes

OPTIONS_DEFINE=	X11 DOCS
OPTIONS_DEFAULT=	X11

OPTIONS_SUB=	yes
X11_USES=	xorg
X11_USE=	XORG=ice,sm,x11,xaw,xext,xmu,xpm,xt
X11_CONFIGURE_WITH=	x

ALL_TARGET=	without_doc
GNU_CONFIGURE=	yes

post-patch:
	@${REINPLACE_CMD} -e \
		'/ALLSUBDIRS/s|$$(DOCSUBDIRS)||g' ${WRKSRC}/Makefile.in

post-install-DOCS-on:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${WRKSRC}/doc/t1lib_doc.pdf ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
