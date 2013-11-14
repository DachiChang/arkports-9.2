# New ports collection makefile for:	php5-composer
# Date created:				2013-11-14
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	php5-composer
PORTVERSION=	1.0.0.a7
CATEGORIES=	arkports
MASTER_SITES=	http://getcomposer.org/download/${MASTER_SITE_SUBDIR}/
MASTER_SITE_SUBDIR=	${PORTVERSION:S/.a/-alpha/}
DISTFILES=	composer.phar

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit dependency manager for PHP

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes
USE_PHP=	yes

do-extract:
	${RM} -rf ${WRKDIR}
	${MKDIR} ${WRKDIR}
	${CP} ${DISTDIR}/composer.phar ${WRKSRC}/

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/composer.phar ${PREFIX}/bin/composer

.include <bsd.port.mk>
