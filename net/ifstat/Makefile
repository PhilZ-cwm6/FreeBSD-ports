PORTNAME=	ifstat
PORTVERSION=	1.1
PORTREVISION=	5
CATEGORIES=	net
MASTER_SITES=	http://gael.roualland.free.fr/${PORTNAME}/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Network interface statistics monitoring tool

GNU_CONFIGURE=	yes
USES=		ssl

OPTIONS_DEFINE=	SNMP
SNMP_LIB_DEPENDS=	libnetsnmp.so:net-mgmt/net-snmp
SNMP_CONFIGURE_WITH=	snmp

PLIST_FILES=	bin/ifstat man/man1/ifstat.1.gz

.include <bsd.port.mk>
