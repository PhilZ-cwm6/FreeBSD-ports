PORTNAME=	DBIx-Log4perl
PORTVERSION=	0.26
PORTREVISION=	1
CATEGORIES=	databases perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	For DBI to selectively log SQL, parameters, result-sets, transactions

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-DBI>=1.500:databases/p5-DBI \
		p5-Log-Log4perl>=1.04:devel/p5-Log-Log4perl

USES=		perl5
USE_PERL5=	configure

.include <bsd.port.mk>
