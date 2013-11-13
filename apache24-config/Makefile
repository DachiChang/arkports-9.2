# New ports collection makefile for:	apache24-config
# Date created:				2013-11-12
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	apache24-config
PORTVERSION=	2.4.6
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit apache24 configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

PLIST_SUB+=	PORT_DBDIR="${PORT_DBDIR}"
PLIST_SUB+=	PKGNAME="${PKGNAME}"

do-install:
	(cd ${FILESDIR}/option; \
		${FIND} . -type d -exec ${MKDIR} ${PORT_DBDIR}/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL} -m 644 \{} ${PORT_DBDIR}/\{} \;)
	(cd ${FILESDIR}/config; \
		${FIND} . -type d -exec ${MKDIR} ${PREFIX}/etc/apache24/Includes/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL_DATA} \{} ${PREFIX}/etc/apache24/Includes/\{} \;)
	PKG_PREFIX=${PREFIX} ${SH} ${PKGINSTALL} ${PKGNAME} DO-INSTALL

.include <bsd.port.mk>
