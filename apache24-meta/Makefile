# New ports collection makefile for:	apache24-meta
# Date created:				2013-11-13
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	apache24-meta
PORTVERSION=	1.0
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit apache24 http server with php5 support

RUN_DEPENDS=	ark-apache24-config>=0:${PORTSDIR}/arkports/apache24-config \
		apache24>=0:${PORTSDIR}/www/apache24 \
		ap24-mod_fcgid>=0:${PORTSDIR}/www/mod_fcgid \
		ark-php5-meta>=0:${PORTSDIR}/arkports/php5-meta

NO_WRKSUBDIR=	yes
NO_BUILD=	yes
NO_STAGE=	yes
NO_PACKAGE=	yes

do-install:
	${DO_NADA}

.include <bsd.port.mk>
