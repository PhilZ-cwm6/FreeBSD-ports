PORTNAME=	SMS-Send-NexmoUnicode
PORTVERSION=	0.02
CATEGORIES=	comms perl5
MASTER_SITES=	CPAN
MASTER_SITE_SUBDIR=	CPAN:JNLIN
PKGNAMEPREFIX=	p5-

MAINTAINER=	jnlin@freebsd.cs.nctu.edu.tw
COMMENT=	SMS::Send driver for www.nexmo.com (Unicode)

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Nexmo-SMS>=0.04:comms/p5-Nexmo-SMS \
		p5-SMS-Send>=0:comms/p5-SMS-Send

USES=		perl5
USE_PERL5=	configure

.include <bsd.port.mk>
