# $FreeBSD$

PORTNAME=	UNIVERSAL-ref
PORTVERSION=	0.14
PORTREVISION=	1
CATEGORIES=	devel perl5
MASTER_SITES=	CPAN
MASTER_SITE_SUBDIR=	CPAN:JJORE
PKGNAMEPREFIX=	p5-

MAINTAINER=	tobez@FreeBSD.org
COMMENT=	Turns ref() into a multimethod

BUILD_DEPENDS=	p5-B-Utils>=0:devel/p5-B-Utils
RUN_DEPENDS:=	${BUILD_DEPENDS}

USES=		perl5
USE_PERL5=	configure

.include <bsd.port.pre.mk>

.if ${PERL_LEVEL} >= 502501
BROKEN=		Does not build, op_sibling usage. https://rt.cpan.org/Public/Bug/Display.html?id=118008
.endif

.include <bsd.port.post.mk>
