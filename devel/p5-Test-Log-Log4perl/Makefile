PORTNAME=	Test-Log-Log4perl
PORTVERSION=	0.32
CATEGORIES=	devel perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Test log4perl

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Log-Log4perl>=0:devel/p5-Log-Log4perl
TEST_DEPENDS=	p5-Test-Exception>=0:devel/p5-Test-Exception

USES=		perl5
USE_PERL5=	configure

NO_ARCH=	yes

.include <bsd.port.mk>
