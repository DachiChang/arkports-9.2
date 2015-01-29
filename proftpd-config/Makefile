# New ports collection makefile for:	proftpd-config
# Date created:				2013-12-22
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	proftpd-config
PORTVERSION=	1.3.4d
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit proftpd configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

do-install:
	${MKDIR} ${PREFIX}/etc
	${INSTALL_DATA} ${FILESDIR}/config/proftpd.conf ${PREFIX}/etc/
	PKG_PREFIX=${PREFIX} ${SH} ${PKGINSTALL} ${PKGNAME} DO-INSTALL

.include <bsd.port.mk>
