PORTNAME=	DoulosSIL
PORTVERSION=	4.112
PORTREVISION=	2
CATEGORIES=	x11-fonts
MASTER_SITES=	http://scripts.sil.org/cms/scripts/render_download.php?&format=file&media_id=${MEDIA_ID}&filename=/ \
		LOCAL/bf

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Doulos SIL TrueType font collection

LICENSE=	OFL11

USES=		fonts zip

MEDIA_ID=	${DISTNAME}${EXTRACT_SUFX}
NO_BUILD=	yes

PLIST_FILES=	${FONTSDIR}/${PORTNAME}-R.ttf

OPTIONS_DEFINE=	DOCS

PORTDOCS=	FONTLOG.txt OFL-FAQ.txt OFL.txt README.txt

SUB_FILES=	pkg-message

do-install:
	@${MKDIR} ${STAGEDIR}${FONTSDIR}
	@(cd ${WRKSRC} ; ${INSTALL_DATA} *.ttf ${STAGEDIR}${FONTSDIR})
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	@(cd ${WRKSRC} ; ${INSTALL_DATA} ${PORTDOCS} ${STAGEDIR}${DOCSDIR})

.include <bsd.port.mk>
