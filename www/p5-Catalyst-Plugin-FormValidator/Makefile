PORTNAME=	Catalyst-Plugin-FormValidator
PORTVERSION=	0.094
PORTREVISION=	1
CATEGORIES=	www perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	FormValidator for Catalyst

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Catalyst-Runtime>=5.80001:www/p5-Catalyst-Runtime \
		p5-Data-FormValidator>=0:textproc/p5-Data-FormValidator \
		p5-MRO-Compat>=0:devel/p5-MRO-Compat \
		p5-Moose>=0.93:devel/p5-Moose

USES=		perl5
USE_PERL5=	configure

.include <bsd.port.mk>
