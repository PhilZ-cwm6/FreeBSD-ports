PORTNAME=	ktp-auth-handler
DISTVERSION=	${KDE_APPLICATIONS_VERSION}
PORTREVISION=	1
CATEGORIES=	net-im kde kde-applications

MAINTAINER=	kde@FreeBSD.org
COMMENT=	KWallet integration module for KDE Telepathy

LICENSE=	LGPL21+
LICENSE_FILE=	${WRKSRC}/COPYING

LIB_DEPENDS=	libtelepathy-qt5.so:net-im/telepathy-qt \
		libKTpCommonInternals.so:net-im/ktp-common-internals  \
		libaccounts-qt5.so:net-im/libaccounts-qt5 \
		libkaccounts.so:net-im/kaccounts-integration \
		libsignon-qt5.so:sysutils/signon-qt5

USES=		compiler:c++11-lang cmake gettext kde:5 pkgconfig \
		qca qt:5 tar:xz
USE_KDE=	completion config coreaddons i18n jobwidgets kdewebkit \
		kio wallet service solid widgetsaddons windowsystem \
		ecm_build
USE_QT=		concurrent core dbus gui network webkit widgets xml \
		buildtools_build qmake_build

OPTIONS_DEFINE=	DOCS

.include <bsd.port.mk>
