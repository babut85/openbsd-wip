# $OpenBSD$

CATEGORIES =		productivity devel
COMMENT =		C library for Google calendar and contacts
DISTNAME =		libgcal-0.9.6
HOMEPAGE =		https://code.google.com/p/libgcal/

SHARED_LIBS =		gcal	0.0

# BSD
PERMIT_PACKAGE_CDROM =	Yes

WANTLIB =		crypto curl idn m ssl xml2 z

MASTER_SITES =		https://libgcal.googlecode.com/files/
EXTRACT_SUFX =		.tar.bz2

CONFIGURE_STYLE =	gnu
CONFIGURE_ARGS =	${CONFIGURE_SHARED}

MODULES =		devel/gettext
BUILD_DEPENDS =		devel/check
LIB_DEPENDS =		net/curl \
			textproc/libxml

SEPARATE_BUILD =	Yes
DEBUG =			-O0 -ggdb

.include <bsd.port.mk>
