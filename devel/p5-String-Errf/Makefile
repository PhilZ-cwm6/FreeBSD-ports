PORTNAME=	String-Errf
PORTVERSION=	0.007
CATEGORIES=	devel perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	geraud@gcu.info
COMMENT=	Simple sprintf-like dialect

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	p5-TimeDate>=0:devel/p5-TimeDate \
		p5-JSON>=0:converters/p5-JSON \
		${RUN_DEPENDS}
RUN_DEPENDS=	p5-Params-Util>=0:devel/p5-Params-Util \
		p5-Sub-Exporter>=0:devel/p5-Sub-Exporter \
		p5-String-Formatter>=0.102081:devel/p5-String-Formatter

USES=		perl5
USE_PERL5=	configure
NO_ARCH=	yes

.include <bsd.port.mk>
