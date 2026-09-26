# Graph Report - Miguel  (2026-09-26)

## Corpus Check
- Corpus is ~11,187 words - fits in a single context window. You may not need a graph.

## Summary
- 59 nodes · 89 edges · 10 communities (6 shown, 4 thin omitted)
- Extraction: 89% EXTRACTED · 11% INFERRED · 0% AMBIGUOUS · INFERRED: 10 edges (avg confidence: 0.86)
- Token cost: 86,351 input · 0 output

## Community Hubs (Navigation)
- Extraction Rules & Audit
- Skill Setup & CLI
- Incremental Updates & Ingest
- Build, Cluster & Report
- Graph Query Tools
- CLAUDE.md Integration
- Graph DB Exports
- GraphML Export
- SVG Export
- Token Benchmark

## God Nodes (most connected - your core abstractions)
1. `Graphify Skill (/graphify)` - 26 edges
2. `--update Incremental Re-extraction` - 11 edges
3. `Step 4 - Build Graph, Cluster, Analyze` - 7 edges
4. `Extraction Subagent Prompt` - 7 edges
5. `Query Graph First Rule` - 6 edges
6. `Part B - Semantic Extraction (parallel subagents)` - 6 edges
7. `graph.json Output` - 6 edges
8. `graphify query (BFS/DFS traversal)` - 6 edges
9. `Project CLAUDE.md graphify Section` - 5 edges
10. `Part A - Structural (AST) Extraction` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Project CLAUDE.md graphify Section` --semantically_similar_to--> `Graphify Skill Registration (.claude/CLAUDE.md)`  [INFERRED] [semantically similar]
  CLAUDE.md → .claude/CLAUDE.md
- `Update Graph After Code Changes Rule` --conceptually_related_to--> `--update Incremental Re-extraction`  [INFERRED]
  CLAUDE.md → .claude/skills/graphify/references/update.md
- `Project CLAUDE.md graphify Section` --implements--> `graphify claude install (CLAUDE.md integration)`  [INFERRED]
  CLAUDE.md → .claude/skills/graphify/references/hooks.md
- `Query Graph First Rule` --references--> `graphify explain`  [EXTRACTED]
  CLAUDE.md → .claude/skills/graphify/references/query.md
- `Query Graph First Rule` --references--> `graphify path (shortest path)`  [EXTRACTED]
  CLAUDE.md → .claude/skills/graphify/references/query.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Graphify Full Build Pipeline** — _claude_skills_graphify_skill_step1_ensure_installed, _claude_skills_graphify_skill_step2_detect_files, _claude_skills_graphify_skill_part_a_structural_extraction, _claude_skills_graphify_skill_part_b_semantic_extraction, _claude_skills_graphify_skill_part_c_merge, _claude_skills_graphify_skill_step4_build_cluster_analyze, _claude_skills_graphify_skill_step4_5_graph_health_check, _claude_skills_graphify_skill_step5_label_communities, _claude_skills_graphify_skill_step6_obsidian_html, _claude_skills_graphify_skill_step9_manifest_cost [EXTRACTED 1.00]
- **Graphify Optional Exports** — _claude_skills_graphify_references_exports_wiki_export, _claude_skills_graphify_references_exports_neo4j_export, _claude_skills_graphify_references_exports_falkordb_export, _claude_skills_graphify_references_exports_svg_export, _claude_skills_graphify_references_exports_graphml_export, _claude_skills_graphify_references_exports_mcp_server [EXTRACTED 1.00]
- **Graph Query Tools (query/path/explain)** — _claude_skills_graphify_references_query_graphify_query, _claude_skills_graphify_references_query_graphify_path, _claude_skills_graphify_references_query_graphify_explain, claude_query_first_rule [EXTRACTED 1.00]

## Communities (10 total, 4 thin omitted)

### Community 0 - "Extraction Rules & Audit"
Cohesion: 0.22
Nodes (11): Discrete Confidence Score Rubric, Extraction Subagent Prompt, Hyperedges, Node ID Format Rule, EXTRACTED/INFERRED/AMBIGUOUS Audit Trail, Honesty Rules, No API Key Required Policy, Part A - Structural (AST) Extraction (+3 more)

### Community 1 - "Skill Setup & CLI"
Cohesion: 0.22
Nodes (10): Graphify Skill Registration (.claude/CLAUDE.md), /graphify Trigger, graphify clone (GitHub repo), graphify extract CLI, graphify merge-graphs (cross-repo), Graphify Skill (/graphify), Interpreter Guard for Subcommands, Step 1 - Ensure graphify Installed / Interpreter Detection (+2 more)

### Community 2 - "Incremental Updates & Ingest"
Cohesion: 0.22
Nodes (10): /graphify add (URL ingest), graphify.ingest.ingest, --watch Folder Watcher (graphify.watch), source_file Verbatim Rule, Post-Commit Auto-Rebuild Hook, build_merge (replace-on-re-extract), detect_incremental, graph_diff (+2 more)

### Community 3 - "Build, Cluster & Report"
Cohesion: 0.24
Nodes (10): Video/Audio Transcription (transcribe_all, Whisper), Whisper Domain Hint Prompt, --cluster-only, Community Detection, God Nodes, GRAPH_REPORT.md, Shrink Guard (#479), Step 2 - Detect Files (+2 more)

### Community 4 - "Graph Query Tools"
Cohesion: 0.39
Nodes (8): graphify MCP Server (graphify.serve), Constrained Query Expansion, graphify explain, graphify path (shortest path), graphify query (BFS/DFS traversal), Fast Path: Existing Graph, graph.json Output, Query Graph First Rule

### Community 5 - "CLAUDE.md Integration"
Cohesion: 0.40
Nodes (5): Wiki Export (--wiki), graphify claude install (CLAUDE.md integration), Project CLAUDE.md graphify Section, Update Graph After Code Changes Rule, Wiki Index Navigation Rule

## Knowledge Gaps
- **14 isolated node(s):** `Step 1 - Ensure graphify Installed / Interpreter Detection`, `Step 4.5 - Graph Health Check`, `Step 6 - Obsidian Vault + HTML Export`, `Interpreter Guard for Subcommands`, `graphify.ingest.ingest` (+9 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 17 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Graphify Skill (/graphify)` connect `Skill Setup & CLI` to `Extraction Rules & Audit`, `Incremental Updates & Ingest`, `Build, Cluster & Report`, `Graph Query Tools`, `CLAUDE.md Integration`?**
  _High betweenness centrality (0.596) - this node is a cross-community bridge._
- **Why does `Part B - Semantic Extraction (parallel subagents)` connect `Extraction Rules & Audit` to `Skill Setup & CLI`, `Incremental Updates & Ingest`?**
  _High betweenness centrality (0.147) - this node is a cross-community bridge._
- **Why does `--update Incremental Re-extraction` connect `Incremental Updates & Ingest` to `Extraction Rules & Audit`, `Skill Setup & CLI`, `Build, Cluster & Report`, `CLAUDE.md Integration`?**
  _High betweenness centrality (0.146) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `--update Incremental Re-extraction` (e.g. with `Step 9 - Save Manifest and Cost Tracker` and `Update Graph After Code Changes Rule`) actually correct?**
  _`--update Incremental Re-extraction` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Step 1 - Ensure graphify Installed / Interpreter Detection`, `Step 4.5 - Graph Health Check`, `Step 6 - Obsidian Vault + HTML Export` to the rest of the system?**
  _14 weakly-connected nodes found - possible documentation gaps or missing edges._