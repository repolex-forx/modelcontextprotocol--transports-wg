# Repolex Knowledge Graph of modelcontextprotocol/transports-wg

RDF knowledge graph data for [modelcontextprotocol/transports-wg](https://github.com/modelcontextprotocol/transports-wg), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download modelcontextprotocol/transports-wg
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── f8a5e86506c859dc7b08dfc9ea81aedbf6d2d8fe
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── f8a5e86506c859dc7b08dfc9ea81aedbf6d2d8fe
│           └── chunk-001.nq.gz
├── blob
│   ├── 00a0a41da3855646d7bffca93b48cf5009c54654.nq.gz
│   ├── 05be64920d58af7194ea336b6fcaffb31fba422d.nq.gz
│   ├── 13e31fd18cbc1c2424179f23c91b470432081f76.nq.gz
│   ├── 1562cb4e901731af8b17db7d89849307ca30a539.nq.gz
│   ├── 185054bef9dfb083b7ab2db43908ffa173a0f48e.nq.gz
│   ├── 3e7a1989d60c7c7da7681db352c5505676949853.nq.gz
│   ├── 41ed26b391998beb1b2df10171e60d277cb46484.nq.gz
│   ├── 47e84ce9a8e05db58c26bf954a7bd5051037d2c2.nq.gz
│   ├── 4b051aea55b8c0a8873171cc0faadb4440318c6f.nq.gz
│   ├── 4ba8d31020d863ecf2c890973697e15492577ad5.nq.gz
│   ├── 50ae92a8585de72f669d906ce2eaa6084f93983e.nq.gz
│   ├── 561c7d1eb771453bca3144cbecef97aa29a081b0.nq.gz
│   ├── 58f32420401f521904d7a08accbf61982d3bfa43.nq.gz
│   ├── 5b944a0bc547d5184cab9565b8b1d75c361893ef.nq.gz
│   ├── 6419466f1bfccb631503c854ee270431d6f998e2.nq.gz
│   ├── 72cb5e06f61390472552d50545cd04bca1e49fd3.nq.gz
│   ├── 77dfc0e6508b532edc8e253f03f5357f3a349b98.nq.gz
│   ├── 8585e61e472bc77ff872ece2097977493c8dd357.nq.gz
│   ├── 8cc38fdd50d9c0998d23f438f28447f62963abed.nq.gz
│   ├── 8e6e07c166fdc0503f59ea0fe13e299770945814.nq.gz
│   ├── 9569b235e789e641d6a60c9f856b3e3d13916438.nq.gz
│   ├── a31002dff57789164fc6afc102158ba3d851719d.nq.gz
│   ├── accbce23f58f41d0178748d1cff1dfab8aea1ac4.nq.gz
│   ├── aee7c682b126004838e5935be51f6a7ab8999737.nq.gz
│   ├── b11a4a8804c02c5e802096af08d9b9f18a1a0671.nq.gz
│   ├── b3d446330a2b192c79f7e9822bd345591eb125db.nq.gz
│   ├── b771ca1e6be0b09e9013a1fd138b96c9c2fc847a.nq.gz
│   ├── c0b43f14f9e172508bdcfc6d874954136ee8b592.nq.gz
│   ├── c1ed23067b7f239e82d3cfb2e9e9dce5186cbb83.nq.gz
│   ├── cd1b0e761ed58df7f079fddcafe07cf6d7b8c5d9.nq.gz
│   ├── d1b1345f05c48557b4fc8713ec157cf8d110e590.nq.gz
│   ├── d2722472ab5208f4d4f944dc8cb0186633ab39c3.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── eccf14d618b445d4e5886899911de20f71cfcddb.nq.gz
│   ├── eeedfc687b4705fb94f64a8a0611d77ed84e5cf8.nq.gz
│   ├── efd43dbd7683ea9ba24fcfba9a6d331aa111999a.nq.gz
│   ├── f5d8661dba580b4cca49862947fe46a295ec4157.nq.gz
│   ├── f5df9446fd2dd8de1673a282123b7149c3a2ebda.nq.gz
│   └── f667b36b774232149eab3a7cce55d8ff63d864a3.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── f8a5e86506c859dc7b08dfc9ea81aedbf6d2d8fe.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 47 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[modelcontextprotocol/transports-wg](https://github.com/modelcontextprotocol/transports-wg)

---
*Parsed on 2026-10-09 by [repolex](https://repolex.ai)*
