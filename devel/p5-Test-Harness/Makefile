PORTNAME=	Test-Harness
PORTVERSION=	3.44
CATEGORIES=	devel perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	Run Perl standard test scripts with statistics

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

NO_ARCH=	yes
USES=		perl5
USE_PERL5=	configure

post-patch:
	@${MV} ${WRKSRC}/bin/prove ${WRKSRC}/bin/p5prove
	@${REINPLACE_CMD} 's|bin/prove|bin/p5prove|' ${WRKSRC}/MANIFEST ${WRKSRC}/Makefile.PL

.include <bsd.port.mk>
