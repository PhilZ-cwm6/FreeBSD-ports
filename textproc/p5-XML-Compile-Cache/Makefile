PORTNAME=	XML-Compile-Cache
PORTVERSION=	1.06
CATEGORIES=	textproc perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	Cache Compiled XML Translators

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Log-Report>=1.26:devel/p5-Log-Report \
		p5-XML-Compile>=1.60:textproc/p5-XML-Compile \
		p5-XML-LibXML-Simple>=0.95:textproc/p5-XML-LibXML-Simple
TEST_DEPENDS=	p5-XML-Compile-Tester>=0.02:devel/p5-XML-Compile-Tester

USES=		perl5
USE_PERL5=	configure
NO_ARCH=	yes

.include <bsd.port.mk>
