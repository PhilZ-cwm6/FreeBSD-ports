PORTNAME=	tty-box
PORTVERSION=	0.7.0
CATEGORIES=	devel rubygems
MASTER_SITES=	RG

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Draw various frames and boxes in your terminal interface

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

RUN_DEPENDS=	rubygem-pastel>=0.8<1:devel/rubygem-pastel \
		rubygem-strings>=0.2.0<0.3:devel/rubygem-strings \
		rubygem-tty-cursor>=0.7<1:devel/rubygem-tty-cursor

USES=		gem
USE_RUBY=	yes

NO_ARCH=	yes

.include <bsd.port.mk>
