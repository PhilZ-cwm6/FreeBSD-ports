PORTNAME=	Apache-DBI
PORTVERSION=	1.12
PORTREVISION=	2
CATEGORIES=	www databases perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	DBI persistent connection, authentication and authorization

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-DBI>=0:databases/p5-DBI \
		${APACHE_PKGNAMEPREFIX}mod_perl2>=0:www/mod_perl2

CONFLICTS=	p5-Apache-DBI-mp[12]*

USES=		apache:2.2+ perl5
USE_PERL5=	configure

.include <bsd.port.mk>
