PORTNAME=	CGI-Application-Plugin-DebugScreen
PORTVERSION=	1.00
PORTREVISION=	1
CATEGORIES=	www perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	bofh@FreeBSD.org
COMMENT=	DebugScreen support for CGI::Application

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-CGI-Application>=0:www/p5-CGI-Application \
		p5-HTML-Template>=0:www/p5-HTML-Template \
		p5-CGI-Application-Plugin-ViewCode>=0:www/p5-CGI-Application-Plugin-ViewCode \
		p5-Devel-StackTrace>=0:devel/p5-Devel-StackTrace \
		p5-UNIVERSAL-require>=0:devel/p5-UNIVERSAL-require

USES=		perl5
USE_PERL5=	configure

.include <bsd.port.mk>
