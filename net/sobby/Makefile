PORTNAME=	sobby
PORTVERSION=	0.4.8
PORTREVISION=	5
CATEGORIES=	net
MASTER_SITES=	http://releases.0x539.de/sobby/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Standalone obby server

LICENSE=	GPLv2

LIB_DEPENDS=	libsigc-2.0.so:devel/libsigc++20 \
		libobby.so:devel/obby \
		libnet6.so:net/net6 \
		libxml++-2.6.so:textproc/libxml++26

USES=		compiler:c++11-lang gnome localbase pkgconfig
USE_CXXSTD=	c++11
USE_GNOME=	glibmm
GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	--disable-zeroconf

PLIST_FILES=	bin/${PORTNAME} man/man1/${PORTNAME}.1.gz

.include <bsd.port.mk>
