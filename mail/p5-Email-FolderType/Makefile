PORTNAME=	Email-FolderType
PORTVERSION=	0.814
CATEGORIES=	mail perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	Determine the type of a mail folder

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-Module-Pluggable>0:devel/p5-Module-Pluggable
TEST_DEPENDS=	p5-Capture-Tiny>0:devel/p5-Capture-Tiny

NO_ARCH=	yes
USES=		perl5
USE_PERL5=	configure

.include <bsd.port.mk>
