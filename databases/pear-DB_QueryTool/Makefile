PORTNAME=	DB_QueryTool
PORTVERSION=	1.1.2
CATEGORIES=	databases www pear

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	PEAR OO-interface for easily retrieving and modifying data in a DB

LICENSE=	BSD2CLAUSE

BUILD_DEPENDS=	${PEARDIR}/DB.php:databases/pear-DB@${PHP_FLAVOR} \
		${PEARDIR}/Log/null.php:sysutils/pear-Log@${PHP_FLAVOR}
RUN_DEPENDS=	${PEARDIR}/DB.php:databases/pear-DB@${PHP_FLAVOR} \
		${PEARDIR}/Log/null.php:sysutils/pear-Log@${PHP_FLAVOR}

USES=		pear

.include <bsd.port.mk>
