PORTNAME=	HTML_Template_Flexy
PORTVERSION=	1.3.13
CATEGORIES=	devel www pear

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Extremely powerful Tokenizer driven Template engine

LICENSE=	PHP202

OPTIONS_DEFINE=	PEAR_HTML_JAVASCRIPT PEAR_FILE_GETTEXT PEAR_TRANSLATION2
PEAR_HTML_JAVASCRIPT_DESC=	PEAR::HTML_Javascript support
PEAR_FILE_GETTEXT_DESC=	PEAR::File_Gettext support
PEAR_TRANSLATION2_DESC=	PEAR::Translation2 support

USES=		pear

PEAR_HTML_JAVASCRIPT_RUN_DEPENDS=	${PEARDIR}/HTML/Javascript.php:devel/pear-HTML_Javascript@${PHP_FLAVOR}
PEAR_FILE_GETTEXT_RUN_DEPENDS=	${PEARDIR}/File/Gettext.php:sysutils/pear-File_Gettext@${PHP_FLAVOR}
PEAR_TRANSLATION2_RUN_DEPENDS=	${PEARDIR}/Translation2.php:sysutils/pear-Translation2@${PHP_FLAVOR}

.include <bsd.port.mk>
