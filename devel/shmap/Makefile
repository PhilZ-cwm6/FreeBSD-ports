PORTNAME=	shmap
PORTVERSION=	0.3.2
PORTREVISION=	2
CATEGORIES=	devel
MASTER_SITES=	SF/${PORTNAME}/${PORTNAME}-devel/${PORTVERSION}

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Shared-memory-based hashmaps

LIB_DEPENDS=	libmm.so:devel/mm

USES=		libtool
GNU_CONFIGURE=	yes
CPPFLAGS+=	-I${LOCALBASE}/include
LDFLAGS+=	-L${LOCALBASE}/lib
USE_LDCONFIG=	yes
CPPFLAGS+=	-D_WANT_SEMUN

post-install:
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/lib/libshmap.so

.include <bsd.port.mk>
