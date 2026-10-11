# Repolex Knowledge Graph of encode/dashboard

RDF knowledge graph data for [encode/dashboard](https://github.com/encode/dashboard), parsed by [repolex](https://repolex.ai).

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
rlex download encode/dashboard
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── a184d749a3a806f8d65574b5712ddce24169c677
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── a184d749a3a806f8d65574b5712ddce24169c677
│           └── chunk-001.nq.gz
├── blob
│   ├── 0588a7d5252cfb181096bd66ada775493cf9ce72.nq.gz
│   ├── 16c2f592a28b69f968631559b02e745667ee962f.nq.gz
│   ├── 1c47d2cc2a5c9de1de2ceed00f1ae3819d579c4f.nq.gz
│   ├── 22f7fbdab0ad0c4fb32f9bc57a23ee8c1c9702df.nq.gz
│   ├── 311b2b56c53f678ab95fc0def708c675d521a807.nq.gz
│   ├── 32b2c4e99b81ab14ab046e64f2fdc48bfcf41136.nq.gz
│   ├── 3f1ef55bb43d318ec18acbdf0ed6d0374ae1d3ef.nq.gz
│   ├── 44899c4b362dc881548e49a5f032afb03a87245b.nq.gz
│   ├── 473cb19b46aafcfa7ffb1fdddb0c6d59dbadb79b.nq.gz
│   ├── 4953e68b3459910df6b0e7d508c58fe4a90fcc18.nq.gz
│   ├── 4ac3beb7a6248488589ae932e29b2d291ca1d55f.nq.gz
│   ├── 51637905c3e971bc6dc042ec9ab0a26e0f5a50af.nq.gz
│   ├── 5750b86927c7b583b8933bfe4eff79df0454796a.nq.gz
│   ├── 632b4d1ca7ff995525e5f1255879d6371aeead5f.nq.gz
│   ├── 720a66392d6260c8535a6e5908f4c0d09412de79.nq.gz
│   ├── 79132734099a8f5b1943f1d8c5e1404570b05852.nq.gz
│   ├── 7bb4bca512f9d0d3e2c17b6ee3f33aa5ac7217b6.nq.gz
│   ├── 7bbd9904f874ca7eac6725c6cda07c6cef8c2992.nq.gz
│   ├── 84284ac36a8f3a6a6caa45afb007ca1fba99ed20.nq.gz
│   ├── 87cc19c276f2d20345dbc1b5f9d88ff2f03e77e2.nq.gz
│   ├── 87ee45e9793ae0a67fcb169d4950aa93e1615ed2.nq.gz
│   ├── 8d71146b4464bd0fab7c06e745be9e3f6eeb6929.nq.gz
│   ├── 9722af02d6459a3cd3a578451098446a95e5f0b8.nq.gz
│   ├── 977acd97d5e0b45d0d23d287f61f2f5a5f012058.nq.gz
│   ├── 9cd5b05bb93b1129b59df3e4ae641beda32261b8.nq.gz
│   ├── a07940013816f76f97b226d850af75304dbef297.nq.gz
│   ├── a1d0395544fdb53accf32ff78e3df5f70ad8abba.nq.gz
│   ├── b502ff97171195af33b45ae05240b8dde1b8ca8c.nq.gz
│   ├── c3907b7e859821c77c1f9c41bdbd5615cd312b76.nq.gz
│   ├── c5653651675d5d12a57734320ba75e7ad66d3ffe.nq.gz
│   ├── c824549184b69274d256ea8eccd72430e41e1e3d.nq.gz
│   ├── dbfd95d0174aa44d3fe5ed0b67dd2670c68b35ec.nq.gz
│   ├── e311350b104a9287fb66ad207e0725699ecd0ed4.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e871360d1642bc3ac222718fa735b9daee6dd0fa.nq.gz
│   ├── f6bd6846a252b4474223c3f62698f53c0746d635.nq.gz
│   ├── f74ed9c32ce2f3b2bef22c7458ed2566fe9abcdf.nq.gz
│   ├── f9309988aeab3868040d3b322658902098eba27f.nq.gz
│   ├── f98177dbf711863eff7c90f84d5d419d02d99ba8.nq.gz
│   ├── fab604866cd5e55ef4525ea22e420c411f510b01.nq.gz
│   ├── fb65357e3e2b2015c7c7fe1f5796f1c6c0c50d45.nq.gz
│   └── fd6e54d612ac45515804782d70c5b32715f0fbb5.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── a184d749a3a806f8d65574b5712ddce24169c677.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 50 files
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

[encode/dashboard](https://github.com/encode/dashboard)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
