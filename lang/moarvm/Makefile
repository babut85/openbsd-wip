# $OpenBSD$

NOT_FOR_ARCHS =		${BE_ARCHS}
SHARED_ONLY =		Yes
BROKEN-arm =		missing atomic ops

COMMENT =		virtual machine for nqp/rakudo

V =			2014.01
DISTNAME =		MoarVM-$V
PKGNAME =		moarvm-$V

SHARED_LIBS =		moar	0.0

CATEGORIES =		lang

HOMEPAGE =		https://github.com/MoarVM/MoarVM/

MAINTAINER =		Pascal Stumpf <Pascal.Stumpf@cubes.de>

# Artistic2
PERMIT_PACKAGE_CDROM =	Yes

WANTLIB =		c kvm m pthread

MASTER_SITES =		http://jnthn.net/MoarVM/

MAKE_FLAGS =		NOISY=1

CONFIGURE_STYLE =	simple
CONFIGURE_SCRIPT =	/usr/bin/perl Configure.pl
CONFIGURE_ARGS +=	--cc="${CC}" --optimize=0 --prefix="${PREFIX}"
CONFIGURE_ENV =		SO_VERSION="${LIBmoar_VERSION}"

NO_TEST =		Yes

.include <bsd.port.mk>
