# New ports collection makefile for:	phpmyadmin-config
# Date created:				2013-11-12
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	phpmyadmin-config
PORTVERSION=	4.0.5
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit phpmyadmin configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

do-install:
	(cd ${FILESDIR}/config; \
		${FIND} . -type d -exec ${MKDIR} ${PREFIX}/etc/apache24/Includes/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL_DATA} \{} ${PREFIX}/etc/apache24/Includes/\{} \;)

.include <bsd.port.mk>
