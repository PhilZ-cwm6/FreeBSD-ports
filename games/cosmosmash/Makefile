PORTNAME=	cosmosmash
DISTVERSION=	1.4.8
CATEGORIES=	games
MASTER_SITES=	http://perso.b2b2c.ca/~sarrazip/dev/ \
		LOCAL/martymac

MAINTAINER=	martymac@FreeBSD.org
COMMENT=	Clone of the Intellivision(TM) game Astrosmash(TM)

LICENSE=	GPLv2

LIB_DEPENDS=	libflatzebra-0.1.so:devel/flatzebra \
		libaa.so:graphics/aalib \
		libmikmod.so:audio/libmikmod \
		libaudiofile.so:audio/libaudiofile

USES=		desktop-file-utils iconv pkgconfig sdl xorg
USE_CXXSTD=	gnu++98
USE_SDL=	image mixer sdl
USE_XORG=	x11 xau xdmcp

GNU_CONFIGURE=	yes

PORTDOCS=	AUTHORS COPYING NEWS README THANKS

OPTIONS_DEFINE=	DOCS

post-patch:
	@${REINPLACE_CMD} 's|^pkgsounddir = .*|pkgsounddir = ${DATADIR}/sounds|' \
		${WRKSRC}/src/Makefile.in
	@${REINPLACE_CMD} 's|^docdir = .*|docdir = ${DOCSDIR}|' \
		${WRKSRC}/Makefile.in

.include <bsd.port.mk>
