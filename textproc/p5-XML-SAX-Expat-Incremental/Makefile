PORTNAME=	XML-SAX-Expat-Incremental
PORTVERSION=	0.05
PORTREVISION=	1
CATEGORIES=	textproc perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	XML::SAX::Expat subclass for non-blocking (incremental)

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-XML-Parser>0:textproc/p5-XML-Parser \
		p5-XML-SAX-Expat>0:textproc/p5-XML-SAX-Expat
TEST_DEPENDS=	p5-Test-Exception>=0:devel/p5-Test-Exception

USES=		perl5
USE_PERL5=	configure

.include <bsd.port.mk>
