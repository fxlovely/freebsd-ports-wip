# $FreeBSD: head/biology/vsearch/Makefile 501148 2019-05-09 22:12:26Z jwb $

PORTNAME=		vsearch
DISTVERSIONPREFIX=	v
DISTVERSION=		2.15.0
CATEGORIES=		wip biology

MAINTAINER=	jwb@FreeBSD.org
COMMENT=	Versatile open-source tool for metagenomics

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

# Note: For PPC need power8 or later, little endian
ONLY_FOR_ARCHS=		aarch64 amd64
ONLY_FOR_ARCHS_REASON=	Explicitly enumerated by upstream developers

LIB_DEPENDS=	libsysinfo.so:devel/libsysinfo

USES=		autoreconf ghostscript:build gmake localbase
USE_GITHUB=	yes

GH_ACCOUNT=	torognes
GNU_CONFIGURE=	yes

PLIST_FILES=	bin/vsearch man/man1/vsearch.1.gz
PORTDOCS=	*

OPTIONS_DEFINE=	DOCS
OPTIONS_SUB=	yes

.include <bsd.port.mk>
