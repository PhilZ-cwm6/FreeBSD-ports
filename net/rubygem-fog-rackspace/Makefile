PORTNAME=	fog-rackspace
PORTVERSION=	0.1.6
CATEGORIES=	net rubygems
MASTER_SITES=	RG

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Module for the 'fog' gem to support Rackspace

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.md

RUN_DEPENDS=	rubygem-fog-core>=1.35:devel/rubygem-fog-core \
		rubygem-fog-json>=1.0:devel/rubygem-fog-json \
		rubygem-fog-xml>=0.1:textproc/rubygem-fog-xml \
		rubygem-ipaddress>=0.8:net/rubygem-ipaddress

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

.include <bsd.port.mk>
