PORTNAME=	MooseX-Runnable
PORTVERSION=	0.10
CATEGORIES=	devel perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Tag a class as a runnable application

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Class-Load>=0:devel/p5-Class-Load \
		p5-List-SomeUtils>=0:devel/p5-List-SomeUtils \
		p5-Moose>=0:devel/p5-Moose \
		p5-MooseX-Getopt>=0:devel/p5-MooseX-Getopt \
		p5-MooseX-Types>=0:devel/p5-MooseX-Types \
		p5-MooseX-Types-Path-Class>=0:devel/p5-MooseX-Types-Path-Class \
		p5-Params-Util>=0:devel/p5-Params-Util \
		p5-Path-Tiny>=0:devel/p5-Path-Tiny \
		p5-namespace-autoclean>=0:devel/p5-namespace-autoclean
TEST_DEPENDS=	p5-Test-Fatal>=0:devel/p5-Test-Fatal \
		p5-Test-TableDriven>=0:devel/p5-Test-TableDriven

USES=		perl5
USE_PERL5=	modbuildtiny

NO_ARCH=	yes

.include <bsd.port.mk>
