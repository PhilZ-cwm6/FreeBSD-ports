PORTNAME=	festvox-ked16
PORTVERSION=	1.4.0
PORTREVISION=	1
CATEGORIES=	audio accessibility
MASTER_SITES=	FESTIVAL/1.4.1
DISTNAME=	festvox_kedlpc16k
DIST_SUBDIR=	festival

MAINTAINER=	ports@FreeBSD.org
COMMENT=	American English male voice, sampled at 16 kHz, for Festival

RUN_DEPENDS=	\
${LOCALBASE}/share/festival/lib/dicts/wsj.wp39.poslexR:audio/festlex-poslex \
${LOCALBASE}/share/festival/lib/dicts/cmu/cmulex.scm:audio/festlex-cmu

WRKSRC=		${WRKDIR}/festival

CONFLICTS=	festvox-ked8

NO_BUILD=	yes

FHOME=		${PREFIX}/share/festival

do-install:
	@${MKDIR} ${STAGEDIR}${FHOME}
	cd ${WRKSRC} && ${COPYTREE_SHARE} . ${STAGEDIR}${FHOME}

.include <bsd.port.mk>
