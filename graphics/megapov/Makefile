PORTNAME=	megapov
PORTVERSION=	1.2.1
PORTREVISION=	8
CATEGORIES=	graphics
MASTER_SITES=	http://megapov.inetart.net/packages/unix/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Unofficial extensions of POV-Ray

DEPRECATED=	Abandoned upstream. graphics/povray37 is the recommended replacement.
EXPIRATION_DATE=	2022-10-01

LIB_DEPENDS=	libpng.so:graphics/png \
		libtiff.so:graphics/tiff
#RUN_DEPENDS=	povray:graphics/povray-meta

INSTALL_WRKSRC=	${WRKSRC}/unix

USES=		compiler:c11 gmake jpeg localbase tar:bzip2
USE_CXXSTD=	c++98
GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	COMPILED_BY="ports@FreeBSD.org"

PORTDOCS=	*
PORTEXAMPLES=	*
PLIST_FILES=	bin/megapov

OPTIONS_DEFINE=		DOCS EXAMPLES OPTIMIZED_CFLAGS X11
OPTIONS_DEFINE_amd64=	SVGALIB
OPTIONS_DEFINE_i386=	SVGALIB

OPTIMIZED_CFLAGS_CFLAGS=\
			-O3 -ffast-math -finline-functions \
			-fomit-frame-pointer -funroll-loops \
			-fexpensive-optimizations
SVGALIB_LIB_DEPENDS=	libvga.so:graphics/svgalib
SVGALIB_CONFIGURE_WITH=	svga
X11_USES=		xorg
X11_USE=		xorg=x11,xpm
X11_CONFIGURE_WITH=	x

post-patch:
	@${REINPLACE_CMD} -e \
		's|"-O3"|""|' ${WRKSRC}/configure

post-install-DOCS-on:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	@(cd ${WRKSRC}/doc && ${COPYTREE_SHARE} . ${STAGEDIR}${DOCSDIR})

post-install-EXAMPLES-on:
	@${MKDIR} ${STAGEDIR}${EXAMPLESDIR}
	@(cd ${WRKSRC} && ${COPYTREE_SHARE} "include scenes" ${STAGEDIR}${EXAMPLESDIR})

.include <bsd.port.mk>
