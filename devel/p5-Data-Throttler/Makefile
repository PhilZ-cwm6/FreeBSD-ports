PORTNAME=	Data-Throttler
PORTVERSION=	0.08
CATEGORIES=	devel perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	markun@onohara.to
COMMENT=	Limit data throughput

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Log-Log4perl>=1:devel/p5-Log-Log4perl \
		p5-Set-IntSpan>0:math/p5-Set-IntSpan \
		p5-Text-ASCIITable>0:textproc/p5-Text-ASCIITable \
		p5-YAML>=0.62:textproc/p5-YAML

NO_ARCH=	yes
USES=		perl5
USE_PERL5=	configure

.include <bsd.port.mk>
