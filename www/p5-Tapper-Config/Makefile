# $OpenBSD $

COMMENT=	context sensitive configuration hub for all Tapper libs	

MODULES=	cpan
DISTNAME=	Tapper-Config-4.1.3
PKGNAME=	p5-${DISTNAME:S/-perl-/-/}
CATEGORIES=	www

MAINTAINER =    Sergey Bronnikov <estetus@gmail.com>

# BSD
PERMIT_PACKAGE_CDROM=	Yes

RUN_DEPENDS=    devel/p5-File-ShareDir \
                devel/p5-File-Slurp \
                devel/p5-Hash-Merge-Simple \
                devel/p5-YAML-Syck

BUILD_DEPENDS=  ${RUN_DEPENDS}

.include <bsd.port.mk>
