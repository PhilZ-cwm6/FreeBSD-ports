PORTNAME=	aee
DISTVERSION=	2.2.22
CATEGORIES=	editors

MAINTAINER=	portmaster@BSDforge.com
COMMENT=	Easy editor with both curses and X11 interfaces

LICENSE=	ART10
LICENSE_FILE=	${WRKSRC}/Artistic

USES=		ncurses
PLIST_FILES=	bin/aee bin/rae man/man1/aee.1.gz ${DATADIR}/help.ae
ALL_TARGET=	main

USE_GITLAB=	yes
GL_ACCOUNT=	ports1
GL_PROJECT=	aee
GL_COMMIT=	bf68f4accb96ac39020ac2d9092022aebfa5df27

OPTIONS_DEFINE=	XAE

XAE_DESC=		Build X11 version 'xae'
XAE_USES=		xorg
XAE_USE=		XORG=x11
XAE_PLIST_FILES=	bin/xae bin/rxae
XAE_ALL_TARGET=		xae
XAE_DESKTOP_ENTRIES=	"Xae" "" "" "xae" "" false

post-patch:
	@${REINPLACE_CMD} -e \
		's|cc|${CC}|g ; \
		 s|"-s"|""|g ; \
		 s|/usr/X11R6|${LOCALBASE}|g' \
		 ${WRKSRC}/create.mk.aee \
		 ${WRKSRC}/create.mk.xae
	@${REINPLACE_CMD} -e 's|/usr/local/lib|${DATADIR}|g' \
		${WRKSRC}/aee.1  \
		${WRKSRC}/localize.c
		${CHMOD} 0544 ${WRKSRC}/create.mk.aee ${WRKSRC}/create.mk.xae ${WRKSRC}/install-sh

do-install:
	@${MKDIR} ${STAGEDIR}${DATADIR}
	${INSTALL_PROGRAM} ${WRKSRC}/aee ${STAGEDIR}${PREFIX}/bin
	(cd ${STAGEDIR}${PREFIX}/bin && ${LN} aee rae)
	${INSTALL_MAN} ${WRKSRC}/aee.1 ${STAGEDIR}${MANPREFIX}/man/man1
	${INSTALL_DATA} ${WRKSRC}/help.ae ${STAGEDIR}${DATADIR}

do-install-XAE-on:
	${INSTALL_PROGRAM} ${WRKSRC}/xae ${STAGEDIR}${PREFIX}/bin
	(cd ${STAGEDIR}${PREFIX}/bin && ${LN} xae rxae)

.include <bsd.port.mk>
