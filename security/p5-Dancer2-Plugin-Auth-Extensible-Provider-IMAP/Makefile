PORTNAME=	Dancer2-Plugin-Auth-Extensible-Provider-IMAP
PORTVERSION=	0.003
CATEGORIES=	security perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	Extensible authentication for D2 apps using Net::IMAP::Simple

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Dancer2-Plugin-Auth-Extensible>=0.620:security/p5-Dancer2-Plugin-Auth-Extensible \
		p5-Net-IMAP-Simple>=0:mail/p5-Net-IMAP-Simple

USES=		perl5
USE_PERL5=	configure
NO_ARCH=	yes

.include <bsd.port.mk>
