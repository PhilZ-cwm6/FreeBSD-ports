PORTNAME=	mailimporter
DISTVERSION=	${KDE_APPLICATIONS_VERSION}
PORTREVISION=	1
CATEGORIES=	net kde kde-applications

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Import mbox files to KMail

LICENSE=	LGPL21

BUILD_DEPENDS=	${LOCALBASE}/include/boost/range/algorithm.hpp:devel/boost-libs

USES=		cmake compiler:c++11-lib gettext kde:5 qt:5 tar:xz
USE_KDE=	auth archive codecs config configwidgets coreaddons i18n itemmodels \
		kio service widgetsaddons \
		ecm_build
# pim components
USE_KDE+=	akonadi akonadimime libkdepim mime pimcommon
USE_QT=		concurrent core dbus gui network uitools widgets xml \
		buildtools_build qmake_build testlib_build
USE_LDCONFIG=	yes

DESCR=		${.CURDIR:H:H}/deskutils/kdepim/pkg-descr

OPTIONS_DEFINE=	DOCS

.include <bsd.port.mk>
