PORTNAME=	dfvfs
PORTVERSION=	20210606
CATEGORIES=	security devel python
MASTER_SITES=	https://github.com/log2timeline/dfvfs/releases/download/${PORTVERSION}/ \
		LOCAL/antoine
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	antoine@FreeBSD.org
COMMENT=	Digital Forensics Virtual File System

LICENSE=	APACHE20
LICENSE_FILE=	${WRKSRC}/LICENSE

RUN_DEPENDS=	libbde>=a:devel/libbde \
		libewf>=0:devel/libewf \
		libfsapfs>=e:devel/libfsapfs \
		libfsext>=e:devel/libfsext \
		libfshfs>=e:devel/libfshfs \
		libfsntfs>=e:devel/libfsntfs \
		libfsxfs>=e:devel/libfsxfs \
		libfvde>=0:sysutils/libfvde \
		libfwnt>=e:devel/libfwnt \
		libluksde>=e:devel/libluksde \
		libmodi>=e:devel/libmodi \
		libqcow>=a:devel/libqcow \
		libsigscan>=e:devel/libsigscan \
		libsmdev>=a:devel/libsmdev \
		libsmraw>=a:devel/libsmraw \
		libvhdi>=e:devel/libvhdi \
		libvmdk>=e:devel/libvmdk \
		libvshadow>=0:devel/libvshadow \
		libvsgpt>=e:devel/libvsgpt \
		libvslvm>=e:devel/libvslvm \
		${PYTHON_PKGNAMEPREFIX}cryptography>=0:security/py-cryptography@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}dfdatetime>=0:security/py-dfdatetime@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}dtfabric>=0:devel/py-dtfabric@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}idna>=0:dns/py-idna@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}pytsk>=0:sysutils/py-pytsk@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}sqlite3>=0:databases/py-sqlite3@${PY_FLAVOR}
TEST_DEPENDS=	${PYTHON_PKGNAMEPREFIX}mock>0:devel/py-mock@${PY_FLAVOR} \
		ca_root_nss>=0:security/ca_root_nss

USES=		python:3.5+
USE_LOCALE=	en_US.UTF-8
USE_PYTHON=	distutils autoplist concurrent

NO_ARCH=	yes

# Upstream archive contains files with UTF-8 names
EXTRACT_CMD=	${SETENV} LC_ALL=en_US.UTF-8 /usr/bin/bsdtar

post-patch:
	${REINPLACE_CMD} "s,share/doc/dfvfs,${DOCSDIR_REL}," ${WRKSRC}/setup.py

do-test:
	@(cd ${TEST_WRKSRC} && ${SETENV} ${TEST_ENV} ${PYTHON_CMD} run_tests.py)

.include <bsd.port.mk>
