PORTNAME=	heroics
PORTVERSION=	0.1.2
CATEGORIES=	www rubygems
MASTER_SITES=	RG

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Ruby HTTP client generator for APIs represented with JSON schema

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

RUN_DEPENDS=	rubygem-erubis>=2.0<3:www/rubygem-erubis \
		rubygem-excon>=0:devel/rubygem-excon \
		rubygem-moneta>=0:devel/rubygem-moneta \
		rubygem-multi_json>=1.9.2:devel/rubygem-multi_json

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

PLIST_FILES=	bin/heroics-generate \
		bin/heroku-api

.include <bsd.port.mk>
