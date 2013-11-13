# New ports collection makefile for:	mysql56-config
# Date created:				2013-11-13
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	mysql56-config
PORTVERSION=	5.6.13
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit mysql56 server configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

PLIST_SUB+=	PKGNAME="${PKGNAME}"

do-install:
	(cd ${FILESDIR}/config; \
		${FIND} . -type d -exec ${MKDIR} ${PREFIX}/etc/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL_DATA} \{} ${PREFIX}/etc/\{} \;)
	PKG_PREFIX=${PREFIX} ${SH} ${PKGINSTALL} ${PKGNAME} DO-INSTALL

.include <bsd.port.mk>
