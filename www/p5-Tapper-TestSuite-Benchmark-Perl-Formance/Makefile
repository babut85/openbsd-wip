# $OpenBSD $

COMMENT=	wrapper for Benchmark::Perl::Formance

MODULES=	cpan
DISTNAME=	Tapper-TestSuite-Benchmark-Perl-Formance-4.1.1
PKGNAME=	p5-${DISTNAME:S/-perl-/-/}
CATEGORIES=	www

# BSD
PERMIT_PACKAGE_CDROM=	Yes

RUN_DEPENDS=    devel/p5-Benchmark-Perl-Formance \
		devel/p5-Data-Structure-Util \
		devel/p5-Data-YAML \
		devel/p5-Devel-Platform-Info

BUILD_DEPENDS=  ${RUN_DEPENDS}

.include <bsd.port.mk>
