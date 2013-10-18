# New ports collection makefile for:	screen-config
# Date created:				2013-10-18
# Whom:					Dachi Chang <femc7488@gmail.com>
#
# $FreeBSD$
#

PORTNAME=	screen-config
PORTVERSION=	4.0.3
CATEGORIES=	arkports
MASTER_SITES=	# none
DISTFILES=	# none

MAINTAINER=	femc7488@gmail.com
COMMENT=	Awesome Rapid Kit screen configure

NO_WRKSUBDIR=	yes
NO_PACKAGE=	yes
NO_STAGE=	yes
NO_BUILD=	yes

PLIST_SUB+=	PORT_DBDIR="${PORT_DBDIR}"

do-install:
	${MKDIR} ${EXAMPLESDIR}
	(cd ${FILESDIR}/option; \
		${FIND} . -type d -exec ${MKDIR} ${PORT_DBDIR}/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL} -m 644 \{} ${PORT_DBDIR}/\{} \;)
	(cd ${FILESDIR}/config; \
		${FIND} . -type d -exec ${MKDIR} ${EXAMPLESDIR}/\{} \; ;\
		${FIND} . -type f -exec ${INSTALL_DATA} \{} ${EXAMPLESDIR}/\{} \;)
	${CHMOD} 555 ${EXAMPLESDIR}/install.sh

.include <bsd.port.mk>
