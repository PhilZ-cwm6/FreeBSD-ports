PORTNAME=	jql
DISTVERSIONPREFIX=	v
DISTVERSION=	5.0.0
CATEGORIES=	textproc

MAINTAINER=	yuri@FreeBSD.org
COMMENT=	JSON Query Language CLI tool built with Rust

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE-MIT

USES=		cargo

USE_GITHUB=	yes
GH_ACCOUNT=	yamafaktory

CARGO_CRATES=	ansi_term-0.12.1 \
		anyhow-1.0.61 \
		async-attributes-1.1.2 \
		async-channel-1.6.1 \
		async-executor-1.4.1 \
		async-global-executor-2.0.3 \
		async-io-1.6.0 \
		async-lock-2.5.0 \
		async-mutex-1.4.0 \
		async-process-1.3.0 \
		async-std-1.12.0 \
		async-task-4.2.0 \
		atomic-waker-1.0.0 \
		atty-0.2.14 \
		autocfg-1.1.0 \
		bitflags-1.3.2 \
		block-buffer-0.10.2 \
		blocking-1.2.0 \
		bstr-0.2.17 \
		bumpalo-3.9.1 \
		cache-padded-1.2.0 \
		cast-0.2.7 \
		cast-0.3.0 \
		cc-1.0.73 \
		cfg-if-1.0.0 \
		clap-2.34.0 \
		clap-3.2.17 \
		clap_lex-0.2.3 \
		colored_json-2.1.0 \
		concurrent-queue-1.2.2 \
		cpufeatures-0.2.2 \
		criterion-0.3.6 \
		criterion-plot-0.4.4 \
		crossbeam-channel-0.5.4 \
		crossbeam-deque-0.8.1 \
		crossbeam-epoch-0.9.8 \
		crossbeam-utils-0.8.8 \
		crypto-common-0.1.6 \
		csv-1.1.6 \
		csv-core-0.1.10 \
		ctor-0.1.22 \
		digest-0.10.3 \
		either-1.6.1 \
		event-listener-2.5.2 \
		fastrand-1.7.0 \
		futures-channel-0.3.21 \
		futures-core-0.3.21 \
		futures-io-0.3.21 \
		futures-lite-1.12.0 \
		generic-array-0.14.6 \
		gloo-timers-0.2.3 \
		half-1.8.2 \
		hashbrown-0.11.2 \
		hermit-abi-0.1.19 \
		indexmap-1.8.1 \
		instant-0.1.12 \
		itertools-0.10.3 \
		itoa-0.4.8 \
		itoa-1.0.1 \
		js-sys-0.3.56 \
		kv-log-macro-1.0.7 \
		lazy_static-1.4.0 \
		libc-0.2.121 \
		log-0.4.16 \
		memchr-2.4.1 \
		memoffset-0.6.5 \
		num-traits-0.2.14 \
		num_cpus-1.13.1 \
		once_cell-1.12.0 \
		oorandom-11.1.3 \
		os_str_bytes-6.0.0 \
		parking-2.0.0 \
		pest-2.2.1 \
		pest_derive-2.2.1 \
		pest_generator-2.2.1 \
		pest_meta-2.2.1 \
		pin-project-lite-0.2.8 \
		pin-utils-0.1.0 \
		plotters-0.3.1 \
		plotters-backend-0.3.2 \
		plotters-svg-0.3.1 \
		polling-2.2.0 \
		proc-macro2-1.0.36 \
		quote-1.0.17 \
		rayon-1.5.3 \
		rayon-core-1.9.2 \
		regex-1.5.5 \
		regex-automata-0.1.10 \
		regex-syntax-0.6.25 \
		rustc_version-0.4.0 \
		ryu-1.0.9 \
		same-file-1.0.6 \
		scopeguard-1.1.0 \
		semver-1.0.7 \
		serde-1.0.136 \
		serde_cbor-0.11.2 \
		serde_derive-1.0.136 \
		serde_json-1.0.83 \
		sha-1-0.10.0 \
		signal-hook-0.3.13 \
		signal-hook-registry-1.4.0 \
		slab-0.4.5 \
		socket2-0.4.4 \
		strsim-0.10.0 \
		syn-1.0.90 \
		termcolor-1.1.3 \
		textwrap-0.11.0 \
		textwrap-0.15.0 \
		thiserror-1.0.32 \
		thiserror-impl-1.0.32 \
		tinytemplate-1.2.1 \
		typenum-1.15.0 \
		ucd-trie-0.1.3 \
		unicode-width-0.1.9 \
		unicode-xid-0.2.2 \
		value-bag-1.0.0-alpha.8 \
		version_check-0.9.4 \
		waker-fn-1.1.0 \
		walkdir-2.3.2 \
		wasm-bindgen-0.2.79 \
		wasm-bindgen-backend-0.2.79 \
		wasm-bindgen-futures-0.4.29 \
		wasm-bindgen-macro-0.2.79 \
		wasm-bindgen-macro-support-0.2.79 \
		wasm-bindgen-shared-0.2.79 \
		web-sys-0.3.56 \
		wepoll-ffi-0.1.2 \
		winapi-0.3.9 \
		winapi-i686-pc-windows-gnu-0.4.0 \
		winapi-util-0.1.5 \
		winapi-x86_64-pc-windows-gnu-0.4.0

PLIST_FILES=	bin/${PORTNAME}

post-install:
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/${PORTNAME}

.include <bsd.port.mk>
