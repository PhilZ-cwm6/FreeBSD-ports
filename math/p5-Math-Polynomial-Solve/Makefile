PORTNAME=	Math-Polynomial-Solve
PORTVERSION=	2.86
CATEGORIES=	math perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	Find the roots of polynomial equations

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Math-Utils>=1.06:math/p5-Math-Utils

NO_ARCH=	yes
USES=		dos2unix perl5
USE_PERL5=	configure

.include <bsd.port.mk>
