PORTNAME=	rubymarshal
PORTVERSION=	1.2.10
CATEGORIES=	devel python
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	amdmi3@FreeBSD.org
COMMENT=	Read and write Ruby-marshalled data

LICENSE=	WTFPL
LICENSE_FILE=	${WRKSRC}/LICENSE

TEST_DEPENDS=	${PYTHON_PKGNAMEPREFIX}hypothesis>=0:devel/py-hypothesis@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pytest-mutagen>=0:devel/py-pytest-mutagen@${PY_FLAVOR}

USE_GITHUB=	yes  # tests are missing from PyPI distribution
GH_ACCOUNT=	d9pouces
GH_PROJECT=	RubyMarshal

USES=		python:3.6+ pytest
USE_PYTHON=	autoplist distutils
NO_ARCH=	yes

.include <bsd.port.mk>
