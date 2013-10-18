# New ports collection makefile for:	portmaster-config
# Date created:				2013-10-18
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	portmaster-config
PORTVERSION=	3.17.1
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit portmaster configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

do-install:
	${MKDIR} ${PREFIX}/etc
	${INSTALL_DATA} ${FILESDIR}/config/portmaster.rc ${PREFIX}/etc/

.include <bsd.port.mk>
