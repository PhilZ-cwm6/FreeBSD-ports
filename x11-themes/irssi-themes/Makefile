PORTNAME=	irssi-themes
PORTVERSION=	2016082001
CATEGORIES=	x11-themes irc
MASTER_SITES=	https://irssi-import.github.io/themes/ \
		LOCAL/ehaupt/${PORTNAME}-${PORTVERSION}/
DIST_SUBDIR=	${PORTNAME}

MAINTAINER=	ehaupt@FreeBSD.org
COMMENT=	Collection of additional irssi themes

RUN_DEPENDS=	irssi:irc/irssi

NO_ARCH=	yes
NO_BUILD=	yes

THEMESDIR_REL=	share/irssi/themes

.include <bsd.port.pre.mk>
.include "${MASTERDIR}/Makefile.inc"

.for f in ${DISTFILES}
PLIST_FILES+=	${THEMESDIR_REL}/${f}
.endfor

do-extract:
	@${MKDIR} ${WRKSRC}
.for f in ${DISTFILES}
	@${CP} ${DISTDIR}/${DIST_SUBDIR}/${f} ${WRKSRC}
.endfor

do-install:
	@${MKDIR} ${STAGEDIR}${PREFIX}/${THEMESDIR_REL}
.for f in ${DISTFILES}
	${INSTALL_DATA} ${WRKSRC}/${f} ${STAGEDIR}${PREFIX}/${THEMESDIR_REL}
.endfor

.include <bsd.port.post.mk>
