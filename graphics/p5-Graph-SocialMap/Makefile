PORTNAME=	Graph-SocialMap
PORTVERSION=	0.13
CATEGORIES=	graphics perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	bofh@FreeBSD.org
COMMENT=	Easy tool to create social network maps

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Graph-Writer-GraphViz>=0:graphics/p5-Graph-Writer-GraphViz \
		p5-Graph>=0:math/p5-Graph \
		p5-Quantum-Superpositions>=0:lang/p5-Quantum-Superpositions \
		p5-Spiffy>=0:devel/p5-Spiffy \
		p5-YAML>=0:textproc/p5-YAML

USES=		perl5
USE_PERL5=	modbuildtiny

.include <bsd.port.mk>
