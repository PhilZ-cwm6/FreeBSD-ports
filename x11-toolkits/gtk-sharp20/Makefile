PORTNAME=	gtk-sharp
PORTVERSION=	2.12.45
PORTREVISION=	3
CATEGORIES=	x11-toolkits
MASTER_SITES=	http://download.mono-project.com/sources/gtk-sharp212/
PKGNAMESUFFIX=	20

MAINTAINER=	mono@FreeBSD.org
COMMENT=	GTK+ and GNOME interfaces for the .NET runtime

LICENSE=	LGPL21
LICENSE_FILE=	${WRKSRC}/COPYING

LIB_DEPENDS=	libfontconfig.so:x11-fonts/fontconfig \
		libfreetype.so:print/freetype2
RUN_DEPENDS=	p5-XML-LibXML>=0:textproc/p5-XML-LibXML

USES=		gmake gnome libtool mono pathfix perl5 pkgconfig shebangfix
USE_LDCONFIG=	yes
USE_GNOME=	cairo gdkpixbuf2 gtk20 libglade2
USE_PERL5=	run
SHEBANG_FILES=	parser/*.pl

GNU_CONFIGURE=	yes
MAKE_ENV=	INSTALL_STRIP_FLAG=${STRIP}

.include <bsd.port.pre.mk>

.if defined(MONO_DEFAULT) && ${MONO_DEFAULT} > 6
BROKEN=		fails to build with Mono version ${MONO_DEFAULT}: 'Range' is an ambiguous reference between 'System.Range' and 'Gtk.Range'
.endif

post-patch:
	@${REINPLACE_CMD} -e 's|glib/.*\.h>|glib.h>|g' \
		${WRKSRC}/glib/glue/*.c

.include <bsd.port.post.mk>
