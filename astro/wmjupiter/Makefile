PORTNAME=	wmjupiter
PORTVERSION=	1.21
PORTREVISION=	1
CATEGORIES=	astro windowmaker

MAINTAINER=	tkuiper@inxsoft.net
COMMENT=	Dockapp that displays information on Jupiter

LICENSE=	GPLv2 BSD3CLAUSE
LICENSE_COMB=	dual

USE_GITHUB=	yes
GH_ACCOUNT=	engerim42

PLIST_FILES=	bin/wmJupiter
USES=		gmake xorg
USE_XORG=	x11 xext xpm

pre-patch:
	@${REINPLACE_CMD} -e 's|values.h|float.h|; s|MAXDOUBLE|DBL_MAX|g' \
		${WRKSRC}/wmJupiter.c

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/wmJupiter ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
