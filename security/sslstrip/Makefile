COMMENT =	tool for performing HTTPS stripping attacks

MODPY_EGG_VERSION =	0.9
DISTNAME =	sslstrip-${MODPY_EGG_VERSION}
APKG = ${DISTNAME}

CATEGORIES =	security

HOMEPAGE =	http://www.thoughtcrime.org/software/sslstrip/

MAINTAINER =	Nigel Taylor <nigel@openbsd.org>

# GPLv3+
PERMIT_PACKAGE_CDROM =	Yes

MASTER_SITES =	http://www.thoughtcrime.org/software/sslstrip/

MODULES =	lang/python
RUN_DEPENDS =	py-twisted-web-*:devel/py-twisted/web

SUBST_VARS += APKG

NO_TEST =	Yes

.include <bsd.port.mk>
