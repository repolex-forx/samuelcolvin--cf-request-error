# Repolex Knowledge Graph of samuelcolvin/cf-request-error

RDF knowledge graph data for [samuelcolvin/cf-request-error](https://github.com/samuelcolvin/cf-request-error), parsed by [repolex](https://repolex.ai).

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
rlex download samuelcolvin/cf-request-error
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── fbe9c4c95332cedd8f37838a43034aae1365983b
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── fbe9c4c95332cedd8f37838a43034aae1365983b
│           └── chunk-001.nq.gz
├── blob
│   ├── 11ef9d37bc7fe3879f64735efe56f8b55c71c2ff.nq.gz
│   ├── 4138168d756e27d0ee0b302b9b5daa0cae9df928.nq.gz
│   ├── 519729651a5674112da0db565b64d821ce86d656.nq.gz
│   ├── 5c7b5d3c7a750a60b91dfbb070153d316893f136.nq.gz
│   ├── 977f64c4edc458ac13f6e8e346d5f62c1e579556.nq.gz
│   ├── 978ecd87b7ce9a38ca48a8647681d3ff8a687866.nq.gz
│   ├── a34518aabecf1eb9ff3570685abb70da7c1c03b8.nq.gz
│   ├── a727df347a129093f0269058a3c2c543a4ae5497.nq.gz
│   ├── b44f13230850c71d8b33c40a7be7dca7161a6961.nq.gz
│   ├── ca1f83e3bc15f54d2139888df96ad37e046e3098.nq.gz
│   ├── d1152674e8c881d066e70538cd09e62abe9cdb01.nq.gz
│   ├── d145fc738c5bf8e997821f9709770d4f9fe8f7c9.nq.gz
│   └── eec99512e2b87312bbf5f1801cc650f25332da1b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── fbe9c4c95332cedd8f37838a43034aae1365983b.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 19 files
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

[samuelcolvin/cf-request-error](https://github.com/samuelcolvin/cf-request-error)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
