# Repolex Knowledge Graph of ansible-community/molecule-hetznercloud

RDF knowledge graph data for [ansible-community/molecule-hetznercloud](https://github.com/ansible-community/molecule-hetznercloud), parsed by [repolex](https://repolex.ai).

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
rlex download ansible-community/molecule-hetznercloud
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 3c8444a346854358a997b7adca220e61d16566ea
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 3c8444a346854358a997b7adca220e61d16566ea
│           └── chunk-001.nq.gz
├── blob
│   ├── 05ea1bca8887b8289033c6a0185d155cac11e73f.nq.gz
│   ├── 08570fd5057513a8c390fea7f5d712d317b07499.nq.gz
│   ├── 09f045606e9d44b874c74927e027616f0515c080.nq.gz
│   ├── 0a041280bd00a9d068f503b8ee7ce35214bd24a1.nq.gz
│   ├── 19b3578a24f3f9da75f471ffb71237a2327006e8.nq.gz
│   ├── 31db109c74bd2d8a49219814c8b9a3f0c0a6dd10.nq.gz
│   ├── 33b3edcd01f83b0837126b2b1b3c4f4f3eca33c6.nq.gz
│   ├── 388632f7c9d1eda47d38fed64992b1fe8c42e911.nq.gz
│   ├── 3dd2d1640e64ff83e5eaaf1e666b3e4f51b33c25.nq.gz
│   ├── 4230ba85d2600e4078246895d8f7ffd28516c3a6.nq.gz
│   ├── 432d0345c17cc97064c205e5184a7d97849fe79f.nq.gz
│   ├── 48a0647f6c2a44cc3fd6e24409b81ab5af2ccc9d.nq.gz
│   ├── 520046fba0b1cff83c2a3a1a2f8a05448dd2f503.nq.gz
│   ├── 6b108f98faaa7147000100638427f8fbecb60df2.nq.gz
│   ├── 776393911c91baf84f33f7068cf8444b8ab860ef.nq.gz
│   ├── 83e49b6af3bef7fa2a162c8f0092acea3373aee2.nq.gz
│   ├── 9de3e3f0424ec3690f62111b948d268e5d63f462.nq.gz
│   ├── 9e9cd92008f7dc863ba05ce7077222688a9471c2.nq.gz
│   ├── a5f725f3c55e6f8f05a4d4e1ef80040edad3b1d0.nq.gz
│   ├── a990b618f660cad1537c5271f492c3a92d4cc961.nq.gz
│   ├── b2e794ae8869c9c31c84f7179d97b9d6c3ce162b.nq.gz
│   ├── b2f52dedc7fa890e72c43bd938104ec4abef7596.nq.gz
│   ├── b44e7e57398816f70627dc8e60b4544e981daf28.nq.gz
│   ├── b501c494fc36d49dee1942fc5fe3343a90ab8b57.nq.gz
│   ├── b7b6451eb8dfaba0018a52e5327f6565bd5659a0.nq.gz
│   ├── be08b70a6970ce1add10da65bc29fc36b7a56b41.nq.gz
│   ├── bf1efc59fcb742dabf9cf2579f7eb1f1543fb708.nq.gz
│   ├── c3c23430f3f63b4297f86de932c48c3aef12d1aa.nq.gz
│   ├── dbbd5f76c472b0c919d1b3d54add1bf990623eef.nq.gz
│   ├── de56fc0d0af34dc6489ad4cd51496ced92539f5d.nq.gz
│   ├── e0bdffacbf745f4fd1dc2fd08659c14d0fd98bf0.nq.gz
│   ├── e1875cce89ce6633b7277a1b1dc29fb53ac4fa25.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e9a32abd9b264390fe0d38f1a5ba9aff3d069883.nq.gz
│   ├── f61f1c7ece31a460dc361f5032ec4e1fd8807c02.nq.gz
│   └── f6bb1209f26dfd38a574edbbcdfea6797f2aeb69.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 3c8444a346854358a997b7adca220e61d16566ea.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 44 files
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

[ansible-community/molecule-hetznercloud](https://github.com/ansible-community/molecule-hetznercloud)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
