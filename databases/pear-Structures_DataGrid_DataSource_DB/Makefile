PORTNAME=	Structures_DataGrid_DataSource_DB
PORTVERSION=	0.1.1
CATEGORIES=	databases www pear

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	DB datasource driver for pear-Structures_DataGrid

LICENSE=	BSD2CLAUSE

RUN_DEPENDS=	${PEARDIR}/Structures/DataGrid.php:devel/pear-Structures_DataGrid@${PHP_FLAVOR} \
		${PEARDIR}/DB.php:databases/pear-DB@${PHP_FLAVOR} \
		${PEARDIR}/Structures/DataGrid/DataSource/Array.php:databases/pear-Structures_DataGrid_DataSource_Array@${PHP_FLAVOR}

USES=		pear

.include <bsd.port.mk>
