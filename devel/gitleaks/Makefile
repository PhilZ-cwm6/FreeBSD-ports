PORTNAME=	gitleaks
DISTVERSIONPREFIX=	v
DISTVERSION=	8.10.0
CATEGORIES=	devel

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	Tool for detecting hardcoded secrets in git repositories

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		go:modules

GO_MODULE=	github.com/zricethezav/gitleaks/v8
GO_TARGET=	.
PLIST_FILES=	bin/${PORTNAME}

.include <bsd.port.mk>
