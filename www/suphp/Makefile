PORTNAME=	suphp
PORTVERSION=	0.7.2
PORTREVISION=	2
CATEGORIES=	www
MASTER_SITES=	http://www.suphp.org/download/ \
		LOCAL/bdrewery/${PORTNAME}/ \
		http://mirror.shatow.net/freebsd/${PORTNAME}/
PKGNAMESUFFIX=	${PHP_PKGNAMESUFFIX}

MAINTAINER=	freebsd-ports@dan.me.uk
COMMENT=	Securely execute PHP scripts under Apache

LICENSE=	GPLv2

GNU_CONFIGURE=	yes
USES=		apache:2.2+ autoreconf cpe libtool php:cgi,flavors
SUB_FILES=	pkg-message

CFLAGS+=	-I${LOCALBASE}/include
USE_CSTD=	gnu89
USE_CXXSTD=	gnu++98

MYPORTDOCS=	apache/CONFIG \
		apache/INSTALL \
		apache/README \
		CONFIG LICENSE \
		INSTALL README

CONFIGURE_ARGS=	CFLAGS="${CFLAGS} -I`${LOCALBASE}/bin/apr-1-config --includedir`" \
		--with-apxs=${APXS}

# WITH_SETID_MODE should be a value of "owner", "force", or "paranoid".
# It's important that you understand the differences between each mode.
# See /usr/local/share/doc/suphp/INSTALL for details.
#
WITH_SETID_MODE?=	owner
CONFIGURE_ARGS+=	--with-setid-mode=${WITH_SETID_MODE}

OPTIONS_DEFINE=	DOCS

.include <bsd.port.options.mk>

CONFIGURE_ARGS+=	--with-apr=${LOCALBASE}

post-install:
.if !defined(WITH_DEBUG)
	@${STRIP_CMD} ${STAGEDIR}${PREFIX}/sbin/suphp
	@${STRIP_CMD} ${STAGEDIR}${PREFIX}/${APACHEMODDIR}/mod_suphp.so
.endif
	${INSTALL_DATA} ${WRKSRC}/doc/suphp.conf-example \
	    ${STAGEDIR}${PREFIX}/etc/suphp.conf-example

post-install-DOCS-on:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}/apache
.for f in ${MYPORTDOCS}
	${INSTALL_DATA} ${WRKSRC}/doc/${f} ${STAGEDIR}${DOCSDIR}/${f}
.endfor

.include <bsd.port.mk>
