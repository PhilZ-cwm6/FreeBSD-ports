PORTNAME=	nss
PORTVERSION=	3.53.1
DISTVERSIONSUFFIX=	-3.el7_9
CATEGORIES=	security linux

MAINTAINER=	emulation@FreeBSD.org
COMMENT=	Network Security Services (Linux CentOS ${LINUX_DIST_VER})

USES=		cpe linux:c7
CPE_VENDOR=	mozilla
USE_LDCONFIG=	yes
USE_LINUX=	nspr sqlite3
USE_LINUX_RPM=	yes

LIB_DISTNAMES=	${DISTNAME} \
		${PORTNAME}-pem-1.0.3-7.el7 \
		${PORTNAME}-softokn-${PORTVERSION}-6.el7_9 \
		${PORTNAME}-util-${PORTVERSION}-1.el7_9
SRC_DISTFILES=	${DISTNAME}${SRC_SUFX}:SOURCE \
		${PORTNAME}-pem-1.0.3-7.el7${SRC_SUFX}:SOURCE \
		${PORTNAME}-softokn-${PORTVERSION}-6.el7_9${SRC_SUFX}:SOURCE \
		${PORTNAME}-util-${PORTVERSION}-1.el7_9${SRC_SUFX}:SOURCE

CONFLICTS=	linux-c6-${PORTNAME}
DESCR=		${.CURDIR}/../${PORTNAME}/pkg-descr

.include <bsd.port.mk>
