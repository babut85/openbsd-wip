# $OpenBSD $

COMMENT=	minimalist object orientation (with Moose compatibility)	

MODULES=	cpan
DISTNAME=	Moo-1.004002
PKGNAME=	p5-${DISTNAME:S/-perl-/-/}
CATEGORIES=	devel

CPAN_AUTHOR=    HAARG

MAINTAINER =    Sergey Bronnikov <estetus@gmail.com>

# Perl
PERMIT_PACKAGE_CDROM=	Yes

RUN_DEPENDS=    devel/p5-Devel-GlobalDestruction \
		devel/p5-Import-Into

BUILD_DEPENDS=  ${RUN_DEPENDS}

.include <bsd.port.mk>
