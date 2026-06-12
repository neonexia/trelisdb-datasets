# trelisdb-datasets

Pre-converted, web-hosted graph datasets for **TrelisDB**. The
`trelisdb datasets load <name>` command fetches these dumps over HTTP and
loads them onto a graph.

Each file is a TrelisDB dump (JSONL: a header line + node/edge frames,
optionally gzip/zstd compressed). They are produced from genuine upstream
sources by the converters in the main repo's `tools/datasets/` (see that
directory's README for provenance + how to regenerate).

| file | dataset |
|---|---|
| `karate.jsonl` | Zachary's Karate Club |
| `movielens-100k.jsonl.gz` | MovieLens 100K |

More (cora, citeseer, pubmed, ogbn-arxiv, wikics, fb15k-237) land here as
they are produced. Large dumps may be added as release assets instead of
committed files.
