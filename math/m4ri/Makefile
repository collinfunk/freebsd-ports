PORTNAME=	M4RI
PORTVERSION=	20240729
DISTVERSIONPREFIX=	release-
CATEGORIES=	math

MAINTAINER=	thierry@FreeBSD.org
COMMENT=	Library for fast arithmetic with dense matrices over F2
WWW=		https://bitbucket.org/malb/m4ri/src/master/

LICENSE=	GPLv2+

LIB_DEPENDS=	libpng.so:graphics/png

USE_GITHUB=	yes
GH_ACCOUNT=	malb
GH_PROJECT=	${PORTNAME:tl}

USES=		autoreconf libtool localbase pkgconfig

GNU_CONFIGURE=	yes
USE_LDCONFIG=	yes
INSTALL_TARGET=	install-strip

.if defined(MAINTAINER_MODE)
TEST_TARGET=	check
# Only needed for tests
USES+=		gmake
.endif

.include <bsd.port.mk>
