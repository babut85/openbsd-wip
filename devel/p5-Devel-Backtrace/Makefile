# $OpenBSD $

COMMENT=	object-oriented backtrace

MODULES=	cpan
DISTNAME=	Devel-Backtrace-0.12
PKGNAME=	p5-${DISTNAME:S/-perl-/-/}
CATEGORIES=	devel

MAINTAINER =    Sergey Bronnikov <estetus@gmail.com>

# Perl
PERMIT_PACKAGE_CDROM=	Yes

RUN_DEPENDS=    devel/p5-Class-Accessor \
		devel/p5-String-Escape

BUILD_DEPENDS=  ${RUN_DEPENDS}

TEST_DEPENDS=	devel/p5-Test-Pod \
		devel/p5-Test-Pod-Coverage

.include <bsd.port.mk>
