PORTNAME=	Tail-Stat
PORTVERSION=	0.26
CATEGORIES=	sysutils perl5
MASTER_SITES=	CPAN
MASTER_SITE_SUBDIR=	CPAN:LONERR
PKGNAMEPREFIX=	p5-

MAINTAINER=	oleg@mamontov.net
COMMENT=	Real-time log statistics server

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-DateTime>=0:devel/p5-DateTime \
		p5-JSON-XS>=0:converters/p5-JSON-XS \
		p5-Log-Dispatch>=2.26:devel/p5-Log-Dispatch \
		p5-POE>=0:devel/p5-POE \
		p5-Pid-File-Flock>=0:devel/p5-Pid-File-Flock \
		p5-Tie-Hash-Indexed>=0:devel/p5-Tie-Hash-Indexed
TEST_DEPENDS=	p5-Test-TCP>=0:devel/p5-Test-TCP

USES=		perl5
USE_PERL5=	configure
NO_ARCH=	yes

USE_RC_SUBR=	tstatd
SUB_LIST+=	RC_SUBR_SUFFIX=${RC_SUBR_SUFFIX}

post-install:
	${MKDIR} ${STAGEDIR}/var/db/tstatd ${STAGEDIR}/var/run/tstatd

.include <bsd.port.mk>
