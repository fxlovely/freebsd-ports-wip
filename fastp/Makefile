# $FreeBSD: head/biology/fastp/Makefile 500737 2019-05-03 14:41:57Z jwb $

PORTNAME=		fastp
DISTVERSIONPREFIX=	v
DISTVERSION=		0.20.1
CATEGORIES=		wip biology

MAINTAINER=	jwb@FreeBSD.org
COMMENT=	Ultra-fast all-in-one FASTQ preprocessor

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		compiler:c++11-lang gmake
USE_GITHUB=	yes

GH_ACCOUNT=	OpenGene

ALL_TARGET=	fastp
PLIST_FILES=	bin/fastp

post-install:
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/fastp

.include <bsd.port.mk>
