# $FreeBSD: head/biology/vt/Makefile 537984 2020-06-05 03:49:53Z linimon $

PORTNAME=	vt
DISTVERSION=	0.57721
CATEGORIES=	wip biology

MAINTAINER=	jwb@FreeBSD.org
COMMENT=	Discovers short variants from Next Generation Sequencing data

LICENSE=	MIT

LIB_DEPENDS=	libhts.so.3:wip/htslib \
		libsvm.so:science/libsvm \
		libdeflate.so:archivers/libdeflate \
		libcurl.so:ftp/curl

USES=		compiler:c++0x gmake ssl
USE_GITHUB=	yes

GH_ACCOUNT=	atks

PLIST_FILES=	bin/vt

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/vt ${STAGEDIR}${PREFIX}/bin

.include <bsd.port.mk>
