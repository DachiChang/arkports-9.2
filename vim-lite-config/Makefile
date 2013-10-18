# New ports collection makefile for:	vim-lite-config
# Date created:				2013-10-18
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	vim-lite-config
PORTVERSION=	7.3.1314
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit vim lite configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

do-install:
	${MKDIR} ${EXAMPLESDIR}
	(cd ${FILESDIR}/config; \
		${FIND} . -type d -exec ${MKDIR} ${EXAMPLESDIR}/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL_DATA} \{} ${EXAMPLESDIR}/\{} \;)
	${CHMOD} 555 ${EXAMPLESDIR}/install.sh

.include <bsd.port.mk>
