# $OpenBSD$

COMMENT =		offline browser
DISTNAME =		httrack-3.47.27

SHARED_LIBS +=  baselinks                 0.0 # 1.0
SHARED_LIBS +=  changecontent             0.0 # 1.0
SHARED_LIBS +=  contentfilter             0.0 # 1.0
SHARED_LIBS +=  displayheader             0.0 # 1.0
SHARED_LIBS +=  filename                  0.0 # 1.0
SHARED_LIBS +=  filename2                 0.0 # 1.0
SHARED_LIBS +=  filenameiisbug            0.0 # 1.0
SHARED_LIBS +=  listlinks                 0.0 # 1.0
SHARED_LIBS +=  log                       0.0 # 1.0
SHARED_LIBS +=  simple                    0.0 # 1.0
SHARED_LIBS +=  htsjava                   0.0 # 2.47
SHARED_LIBS +=  httrack                   0.0 # 2.47

CATEGORIES =		www

HOMEPAGE =		http://www.httrack.com/

# GPLv3+
PERMIT_PACKAGE_CDROM =	Yes

WANTLIB =  c crypto pthread ssl z

MASTER_SITES =		http://mirror.httrack.com/

MODULES =		converters/libiconv

RUN_DEPENDS =		devel/desktop-file-utils \
			x11/gtk+2,-guic

SEPARATE_BUILD =	No
CONFIGURE_STYLE =	gnu autoconf
CONFIGURE_ARGS +=	${CONFIGURE_SHARED} \
			--enable-online-unit-tests=no \
			ICONV_LIBS="-liconv"
CONFIGURE_ENV =		CFLAGS="${CFLAGS} -I${LOCALBASE}/include" \
			LDFLAGS="${LDFLAGS} -L${LOCALBASE}/lib"

AUTOCONF_VERSION =	2.69

pre-configure:
	perl -pi \
		-e '$$. == 1 && s|/bin/bash|/bin/sh|;' \
		-e 'close ARGV if eof;' \
		${WRKSRC}/tests/*.test

.include <bsd.port.mk>
