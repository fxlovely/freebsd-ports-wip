# Created by: Bartek Rutkowski <ports@robakdesign.com>
# $FreeBSD: head/devel/py-click/Makefile 496503 2019-03-21 19:41:43Z sunpoet $

PORTNAME=	click
PORTVERSION=	7.1.1
CATEGORIES=	wip devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
# DISTNAME=	Click-${PORTVERSION}

MAINTAINER=	robak@FreeBSD.org
COMMENT=	Python package for creating command line interfaces

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE.rst

TEST_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pytest>0:devel/py-pytest@${PY_FLAVOR}

USES=		python
USE_PYTHON=	distutils autoplist

NO_ARCH=	yes

do-test:
	@cd ${WRKSRC} && ${PYTHON_CMD} -m pytest -v -p no:warnings

.include <bsd.port.mk>
