# $OpenBSD$

COMMENT =		file system exerciser

DISTNAME =		fsx-0.1
PKGNAME =		${DISTNAME}

CATEGORIES =		sysutils

HOMEPAGE =		http://codemonkey.org.uk/projects/fsx/

MAINTAINER =		Sergey Bronnikov <estetus@gmail.com>

# APPLE PUBLIC SOURCE LICENSE
PERMIT_PACKAGE_CDROM =	Yes

MASTER_SITES =		http://codemonkey.org.uk/projects/fsx/

DISTFILES =		dfly-fsx.c
DIST_SUBDIR =		${DISTNAME}
EXTRACT_ONLY =

NO_TEST =		Yes

WRKDIST =		${WRKDIR}

do-extract:
	cp ${FULLDISTDIR}/${DISTFILES} ${WRKSRC}

do-build:
	cd ${WRKSRC}; \
	${CC} ${CPPFLAGS} -Wall ${CFLAGS} ${LDFLAGS} ${DISTFILES} -o fsx

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/fsx ${PREFIX}/bin/

.include <bsd.port.mk>
