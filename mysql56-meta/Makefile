# New ports collection makefile for:	mysql56-meta
# Date created:				2013-11-13
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	mysql56-meta
PORTVERSION=	1.0
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit mysql56 database server

RUN_DEPENDS=	ark-mysql56-config>=0:${PORTSDIR}/arkports/mysql56-config \
		mysql-server>=0:${PORTSDIR}/databases/mysql56-server

NO_WRKSUBDIR=	yes
NO_BUILD=	yes
NO_STAGE=	yes
NO_PACKAGE=	yes

do-install:
	${DO_NADA}

.include <bsd.port.mk>
