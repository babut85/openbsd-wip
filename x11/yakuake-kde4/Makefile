# $OpenBSD$

CATEGORIES =	x11 sysutils
COMMENT =	quake-style terminal emulator for KDE 4
HOMEPAGE =	http://yakuake.kde.org/
VERSION =	2.9.9
DISTNAME =	yakuake-${VERSION}

MASTER_SITES =	${MASTER_SITE_KDE:=stable/yakuake/${VERSION}/src/}
EXTRACT_SUFX =	.tar.xz

# GPLv2+
PERMIT_PACKAGE_CDROM =          Yes

MODULES =	devel/gettext x11/kde4

WANTLIB =  c m pthread stdc++ X11
WANTLIB += lib/qt4/QtDBus lib/qt4/QtGui lib/qt4/QtNetwork lib/qt4/QtSvg
WANTLIB += lib/qt4/QtXml kdeui kio knewstuff3 knotifyconfig kparts nepomuk
WANTLIB += nepomukutils soprano

RUN_DEPENDS =	${MODKDE4_DEP_DIR}/konsole \
		devel/desktop-file-utils \
		x11/gtk+2,-guic

SUBST_VARS =	PKGNAME

.include <bsd.port.mk>
