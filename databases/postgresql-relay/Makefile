PORTNAME=	postgresql-relay
PORTVERSION=	1.3.2
PORTREVISION=	1
CATEGORIES=	databases net
MASTER_SITES=	http://www.mavetju.org/download/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Multiplex multiple PostgreSQL databases to one relay

LICENSE=	BSD2CLAUSE # from website

USES=		perl5
USE_PERL5=	build
USE_RC_SUBR=	postgresql-relay

PLIST_FILES=	bin/postgresql-relay etc/postgresql-relay.conf-sample \
		man/man8/postgresql-relay.8.gz

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/postgresql-relay ${STAGEDIR}${PREFIX}/bin
	${INSTALL_DATA} ${WRKSRC}/postgresql-relay.conf-sample \
		${STAGEDIR}${PREFIX}/etc/postgresql-relay.conf-sample
	${INSTALL_MAN} ${WRKSRC}/postgresql-relay.8 \
		${STAGEDIR}${MANPREFIX}/man/man8

.include <bsd.port.mk>
