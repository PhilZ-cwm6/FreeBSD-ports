PORTNAME=	RgoogleMaps
PORTVERSION=	1.4.5.3
PORTREVISION=	1
CATEGORIES=	www
DISTNAME=	${PORTNAME}_${PORTVERSION}

MAINTAINER=	tota@FreeBSD.org
COMMENT=	Overlays on Google map tiles in R

LICENSE=	GPLv2+

CRAN_DEPENDS=	R-cran-png>0:graphics/R-cran-png \
		R-cran-sp>0:math/R-cran-sp
RUN_DEPENDS=	${CRAN_DEPENDS}
BUILD_DEPENDS=	${CRAN_DEPENDS}

USES=	cran:auto-plist

.include <bsd.port.mk>
