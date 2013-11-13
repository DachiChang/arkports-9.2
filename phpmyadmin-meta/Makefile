# New ports collection makefile for:	phpmyadmin-meta
# Date created:				2013-11-13
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	phpmyadmin-meta
PORTVERSION=	1.0
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit phpmyadmin

RUN_DEPENDS=	ark-phpmyadmin-config>=0:${PORTSDIR}/arkports/phpmyadmin-config \
		ark-mysql56-meta>=0:${PORTSDIR}/arkports/mysql56-meta \
		ark-apache24-meta>=0:${PORTSDIR}/arkports/apache24-meta \
		phpMyAdmin>=0:${PORTSDIR}/databases/phpmyadmin

NO_WRKSUBDIR=	yes
NO_BUILD=	yes
NO_STAGE=	yes
NO_PACKAGE=	yes

do-install:
	${DO_NADA}

.include <bsd.port.mk>
