# $OpenBSD: Makefile,v 1.4 2013/08/07 21:32:11 naddy Exp $

COMMENT =		computer algebra system (CAS) in Python

MODPY_EGG_VERSION =	0.7.3
DISTNAME =		sympy-${MODPY_EGG_VERSION}
PKGNAME =		py-sympy-${MODPY_EGG_VERSION}
CATEGORIES =		math

HOMEPAGE =		http://sympy.org

MAINTAINER =		Wen Heping <wenheping@gmail.com>

# New BSD
PERMIT_PACKAGE_CDROM =	Yes

MASTER_SITES =		https://github.com/sympy/sympy/releases/download/sympy-${MODPY_EGG_VERSION}/

MODULES =		lang/python
RUN_DEPENDS =		devel/ipython
PATCHORIG =		.origy

do-test:
	        cd ${WRKSRC} && ${MODPY_BIN} setup.py test

.include <bsd.port.mk>
