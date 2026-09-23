# Graph Report - url-ad  (2026-09-23)

## Corpus Check
- 3 files · ~229 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 12 nodes · 10 edges · 4 communities (3 shown, 1 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `349d7ce0`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Roadblocks — URL → Nine Ads (Krea 2 Colab)
- url-ad
- DEMO_URLS.md

## God Nodes (most connected - your core abstractions)
1. `Roadblocks — URL → Nine Ads (Krea 2 Colab)` - 5 edges
2. `url-ad` - 3 edges
3. `Colab (run this)` - 1 edges
4. `Docs` - 1 edges
5. `Demo product URLs` - 1 edges
6. `Model / edit path` - 1 edges
7. `Runtime` - 1 edges
8. `Extraction` - 1 edges
9. `Quality` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Communities (4 total, 1 thin omitted)

### Community 0 - "Roadblocks — URL → Nine Ads (Krea 2 Colab)"
Cohesion: 0.40
Nodes (5): Extraction, Model / edit path, Quality, Roadblocks — URL → Nine Ads (Krea 2 Colab), Runtime

### Community 1 - "url-ad"
Cohesion: 0.67
Nodes (3): Colab (run this), Docs, url-ad

## Knowledge Gaps
- **7 isolated node(s):** `Colab (run this)`, `Docs`, `Demo product URLs`, `Model / edit path`, `Runtime` (+2 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Roadblocks — URL → Nine Ads (Krea 2 Colab)` connect `Roadblocks — URL → Nine Ads (Krea 2 Colab)` to `README.md`?**
  _High betweenness centrality (0.473) - this node is a cross-community bridge._
- **Why does `url-ad` connect `url-ad` to `README.md`?**
  _High betweenness centrality (0.273) - this node is a cross-community bridge._
- **What connects `Colab (run this)`, `Docs`, `Demo product URLs` to the rest of the system?**
  _7 weakly-connected nodes found - possible documentation gaps or missing edges._