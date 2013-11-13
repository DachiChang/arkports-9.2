# New ports collection makefile for:	system-utility-meta
# Date created:				2012-11-13
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	system-utility-meta
PORTVERSION=	1.0
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit system utility tool set

RUN_DEPENDS=	htop>=0:${PORTSDIR}/sysutils/htop \
		tree>=0:${PORTSDIR}/sysutils/tree \
		curl>=0:${PORTSDIR}/ftp/curl \
		rsync>=0:${PORTSDIR}/net/rsync

NO_WRKSUBDIR=	yes
NO_BUILD=	yes

do-install:
	${DO_NADA}

.include <bsd.port.mk>
