# New ports collection makefile for:	php5-config
# Date created:				2013-11-13
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	php5-config
PORTVERSION=	5.4.17
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit php5 and php5-extension configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

PLIST_SUB+=	PORT_DBDIR="${PORT_DBDIR}"

do-install:
	(cd ${FILESDIR}/option; \
		${FIND} . -type d -exec ${MKDIR} ${PORT_DBDIR}/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL} -m 644 \{} ${PORT_DBDIR}/\{} \;)
	(cd ${FILESDIR}/config; \
		${FIND} . -type d -exec ${MKDIR} ${PREFIX}/etc/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL_DATA} \{} ${PREFIX}/etc/\{} \;)

.include <bsd.port.mk>
