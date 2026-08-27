# Awesome-Query-Performance-Optimization

Edit
Top Query Performance Optimization Platforms Ecosystem

Curated List of SaaS Products & Open-Source GitHub Projects
Focused on SQL Query Optimization, Database Performance Monitoring, Query Plans, Index Tuning & Workload Analysis
Last updated: August 2026

This repository tracks notable SaaS/hosted platforms and open-source projects for Query Performance Optimization. These tools help database teams identify slow queries, analyze execution plans, detect regressions, recommend indexes, optimize SQL statements, diagnose database bottlenecks, monitor workloads, and continuously improve database performance.

Examples include EverSQL, pganalyze, Postgres.ai, SolarWinds Database Performance Analyzer, Redgate SQL Monitor, Devart dbForge Monitor, Datadog Database Monitoring, ClusterControl, Percona Toolkit, and SQL Sentry.

Open-source emphasis: This section is heavily expanded with PostgreSQL, MySQL/MariaDB, and cross-database open-source performance tools, extensions, query analyzers, workload profilers, index advisors, database monitoring systems, and tuning utilities. PostgreSQL's ecosystem is particularly strong, with projects such as pg_stat_monitor, pgBadger, PoWA, pg_qualstats, pg_stat_kcache, pgMustard-related tooling, and PostgreSQL's native statistics infrastructure providing substantial building blocks for a self-hosted query optimization stack.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

Table of Contents

SaaS/Hosted Platforms

Open-Source GitHub Projects

Additional Strong Open-Source Options

How to Contribute

Disclaimer

## SaaS / Hosted Platforms

| Product | Core Capabilities | Supported Databases | Pricing (Starting Tier) | Free Tier & Trial Limits |
| :--- | :--- | :--- | :--- | :--- |
| **[pganalyze](https://pganalyze.com)** | PostgreSQL performance monitoring, execution plan analysis, Index Advisor, VACUUM Advisor, and query troubleshooting. | PostgreSQL | Starts at **$149 / month** (Production plan for 1 server, 14 days history; Scale plan at $399/month for up to 4 servers) | **14-day free trial** (Full access, unlimited users, no credit card required; no permanent free tier) |
| **[EverSQL](https://www.eversql.com)** | AI-driven SQL query optimizer and indexing recommendations for automated query rewriting and slow-query tuning. | PostgreSQL, MySQL, MariaDB | **$0** (Free standalone web query optimizer); continuous monitoring starts at **$29 / month** (Aiven platform tiers) | **Free-forever plan** (Unlimited single-query optimizations via web tool) and **14-day free trial** on cloud platform |
| **[pgMustard](https://www.pgmustard.com)** | Visual execution plan analysis for PostgreSQL `EXPLAIN (ANALYZE, BUFFERS)` output with performance tips and bottleneck scoring. | PostgreSQL | Starts at **€95 / year** (~$100/yr for Pro single user; €500/year for Team up to 20 users) | **Free trial: 5 query plan reviews** (Includes all tips and visual plan tree inspection; no credit card required) |
| **[Postgres.ai](https://postgres.ai)** | PostgreSQL development and performance platform with Database Lab Engine (thin database branching/cloning) and automated AI checkups. | PostgreSQL | **$0 / month** (Hobby plan); Express plan starts at **$16 / cluster / month**; DBLab Standard from **$62 / month** | **Free-forever Hobby plan** (Includes weekly AI-assisted database checkup reports for personal/pet projects) |
| **[Datadog Database Monitoring](https://www.datadoghq.com/product/database-monitoring/)** | Enterprise database observability and telemetry correlation with query metrics, execution plans, and wait event analysis. | PostgreSQL, MySQL, SQL Server, Oracle, Aurora | Starts at **$70 / database host / month** (Annual commitment) or **$84 / database host / month** (On-demand) | **14-day free trial** (Full platform access including Database Monitoring, APM, and host metrics; no permanent free tier) |
| **[SolarWinds Database Performance Analyzer (DPA)](https://www.solarwinds.com/database-performance-analyzer)** | Multi-database wait-time analysis, SQL bottleneck identification, blocking/deadlock diagnostics, and anomaly detection. | SQL Server, Oracle, PostgreSQL, MySQL, DB2, SAP ASE | Starts at **$1,699 per database instance** (Perpetual license with 1st yr maintenance) or **$840 / instance / year** (Subscription) | **14-day free trial** (Fully functional across all supported database engines without instance limits) |
| **[SolarWinds SQL Sentry](https://www.solarwinds.com/sql-sentry)** | SQL Server workload profiling, execution plan analysis, tempdb monitoring, deadlock diagnostics, and automated tuning. | SQL Server, Azure SQL | Starts at **$1,233 / target instance / year** (Subscription) or perpetual license starting at **$2,495 / instance** | **14-day free trial** (Fully functional monitoring and diagnostics for SQL Server and cloud database targets) |
| **[Redgate SQL Monitor](https://www.red-gate.com/products/dba/sql-monitor/)** | Fleet-wide SQL Server health monitoring, blocking and deadlock analysis, slow query tracking, and execution plan diagnostics. | SQL Server, Azure SQL | Starts at **$1,233 / server / year** (Standard tier for 1–4 servers; volume discounts starting at 5+ servers) | **14-day free trial** (Full enterprise monitoring feature set across on-premise, virtual machines, and cloud instances) |
| **[ClusterControl](https://severalnines.com/clustercontrol/)** | Multi-database operations, topology deployment, automated failover, query performance monitoring, and backup automation. | MySQL, MariaDB, PostgreSQL, MongoDB, Redis | **€0** (Community Edition); Advanced tier starts at **€250 / node / month** (or **€0.35 / node / hour**) | **Free-forever Community Edition** (Core deployment, monitoring, and replication management) + **30-day free trial** of Enterprise features |
| **[Devart dbForge Studio / Monitor](https://www.devart.com/dbforge/)** | Database IDE and performance monitoring tooling with query profiling, execution plan inspection, and server health tracking. | SQL Server, MySQL, MariaDB, PostgreSQL, Oracle | **$0** (dbForge Monitor add-in for SSMS); dbForge Studio Standard starts at **$119.40 / user / year** (MySQL) or **$229.95 / user / year** (SQL Server) | **30-day free trial** (Enterprise features) which reverts to **free-forever Express Edition** (Basic query editing and management); SSMS Monitor add-in is free forever |
| **[Releem](https://releem.com)** | Automated database configuration tuning, query analytics, and index recommendations via lightweight agent and cloud console. | MySQL, MariaDB, PostgreSQL | Starts at **$11 / server / month** (Hosting plan) or **$25 / server / month** (Advanced plan with query analytics) | **14-day free trial** (Full feature set) and **Free plan** (Basic configuration recommendations for up to 1 server) |

Open-Source GitHub Projects

pg_stat_monitor
Open-source PostgreSQL query-performance monitoring extension developed by Percona. It provides query execution and planning statistics, time buckets, multidimensional query grouping, query plans, table-access statistics, histograms, and other performance information.

pg_stat_statements
PostgreSQL's standard query-statistics extension for collecting execution statistics for SQL statements, providing one of the fundamental data sources for slow-query analysis and optimization.

pgBadger
Fast PostgreSQL log analyzer that generates detailed performance reports from PostgreSQL logs, helping identify slow queries, workload patterns, checkpoints, connections, and database activity.

PoWA
PostgreSQL Workload Analyzer providing a framework for collecting, aggregating, and visualizing PostgreSQL performance statistics from extensions such as pg_stat_statements, pg_qualstats, pg_stat_kcache, and pg_wait_sampling.

pg_qualstats
PostgreSQL extension collecting statistics about query predicates and clauses, useful for identifying columns and predicates that may benefit from indexing or query optimization.

pg_stat_kcache
PostgreSQL extension providing operating-system-level CPU and I/O statistics associated with database activity, helping correlate query workloads with resource consumption.

pg_wait_sampling
PostgreSQL extension for sampling wait events and providing visibility into database contention and wait behavior.

PostgreSQL
The PostgreSQL source tree itself contains extensive native statistics, planner, optimizer, EXPLAIN, and diagnostic capabilities that form the foundation for many query-optimization tools.

MySQL
Open-source MySQL server containing the optimizer, Performance Schema, optimizer tracing, execution-plan infrastructure, and other native mechanisms for query performance analysis.

MariaDB
Open-source relational database with optimizer diagnostics, Performance Schema-compatible instrumentation, query profiling, and database performance tooling.

Percona Server for MySQL
Open-source MySQL-compatible database distribution with additional performance and observability capabilities for demanding database workloads.

Percona Server for PostgreSQL
Open-source PostgreSQL distribution enhanced with Percona tooling and extensions for operational and performance use cases.

Releem Agent
Open-source database advisor agent supporting MySQL, MariaDB, and PostgreSQL. It analyzes database metrics, configuration, indexes, and query execution statistics and can provide automated optimization recommendations.

pg_activity
Terminal-based PostgreSQL activity monitor providing real-time visibility into sessions, queries, CPU, memory, I/O, locks, and database activity.

pg_top
PostgreSQL-oriented top-like monitoring utility for inspecting database activity and identifying resource-intensive sessions and queries.

pgFormatter
SQL/PLpgSQL formatter that makes complex SQL easier to inspect, review, compare, and optimize.

pg_hint_plan
PostgreSQL extension allowing optimizer hints to influence query planning, useful for controlled performance experiments and specialized tuning scenarios.

HypoPG
PostgreSQL extension for hypothetical indexes and other hypothetical database objects, allowing database engineers to evaluate potential indexing strategies without immediately creating physical indexes.

pg_repack
PostgreSQL extension for rebuilding tables and indexes with reduced locking, useful when table/index bloat contributes to performance degradation.

pg_squeeze
PostgreSQL extension designed to reduce table bloat online by reorganizing tables while minimizing application disruption.

Postgres Operator
Open-source PostgreSQL management system that can provide the operational foundation for monitoring, tuning, backups, replication, and performance experimentation.

Prometheus
Open-source monitoring and time-series platform commonly used as the metrics backbone for database performance monitoring.

Grafana
Open-source visualization and observability platform widely used to build database performance dashboards from Prometheus and other metrics sources.

postgres_exporter
Prometheus exporter for PostgreSQL metrics, enabling database statistics to be collected and visualized through Prometheus/Grafana stacks.

Additional Strong Open-Source Options

pg_stat_monitor — Advanced PostgreSQL query-performance monitoring with time buckets, query plans, histograms, and multidimensional statistics.

pg_stat_statements — Core PostgreSQL query statistics.

pgBadger — High-performance PostgreSQL log analysis.

PoWA — PostgreSQL workload analysis framework.

pg_qualstats — Predicate and clause statistics for indexing analysis.

pg_stat_kcache — CPU and I/O statistics for PostgreSQL workloads.

pg_wait_sampling — Wait-event sampling and contention analysis.

HypoPG — Hypothetical indexes for evaluating indexing strategies.

pg_hint_plan — Query-planner hinting and controlled optimization experiments.

pg_activity — Real-time PostgreSQL activity monitoring.

pg_top — Terminal-based PostgreSQL workload monitor.

pg_repack — Online table/index reorganization.

Releem Agent — Open-source automated database advisor for MySQL, MariaDB, and PostgreSQL.

Prometheus — Metrics collection and alerting foundation.

Grafana — Open-source performance visualization layer.

postgres_exporter — PostgreSQL-to-Prometheus metrics bridge.

Percona Toolkit — Although primarily distributed as a tooling suite rather than one database engine, it remains an important open-source collection of database diagnostics and optimization utilities.

Important distinction: There are substantially more open-source database observability and diagnostic components than complete open-source equivalents of pganalyze, EverSQL, SolarWinds DPA, SQL Sentry, or Datadog Database Monitoring. PostgreSQL in particular has an unusually rich ecosystem of extensions for query statistics, waits, predicates, I/O, indexing, logging, and workload analysis.

The strongest open-source strategy is therefore to assemble a modular query-optimization platform:

Database → Query Statistics → Slow Query Detection → EXPLAIN/Plan Collection → Workload Analysis → Index Analysis → Query Rewrite → Benchmarking → Regression Detection → Alerting

A practical PostgreSQL architecture could use:

pg_stat_monitor + pg_stat_statements + pgBadger + PoWA + pg_qualstats + pg_stat_kcache + HypoPG + Prometheus + Grafana

This provides many of the fundamental capabilities required to build a self-hosted alternative to commercial database-performance platforms. pg_stat_monitor, for example, adds time-bucketed and multidimensional query statistics and can expose query plans, histograms, and table-access information.

A more advanced architecture can add:

Slow Query Detection — identify queries consuming excessive execution time, CPU, I/O, or database resources.

Query Fingerprinting — normalize similar SQL statements and aggregate their workload statistics.

Execution Plan Analysis — collect and compare EXPLAIN / EXPLAIN ANALYZE plans.

Plan Regression Detection — detect when a query changes from a fast plan to a slower one.

Index Recommendation — identify missing, unused, redundant, or inefficient indexes.

Hypothetical Index Testing — evaluate potential indexes before deploying them using HypoPG.

Predicate Analysis — use pg_qualstats to understand which query predicates are most important for indexing.

Wait Analysis — identify lock contention, I/O waits, CPU pressure, and other bottlenecks.

CPU/I/O Attribution — correlate database queries with operating-system resource consumption.

Query Rewriting — identify inefficient joins, subqueries, sorting, filtering, aggregation, and other SQL patterns.

Configuration Tuning — optimize database settings based on workload characteristics.

Bloat Analysis — identify table/index bloat and vacuum-related performance problems.

Benchmarking — compare query variants and database configurations before deployment.

Regression Testing — automatically test important queries against new schema, index, or application versions.

Observability — combine database metrics with application, infrastructure, and distributed-tracing telemetry.

Alerting — notify teams when query latency, execution plans, waits, CPU, I/O, or workload characteristics deteriorate.

A strong self-hosted query-performance architecture can therefore look like:

Application → Database → Query Statistics → Query Fingerprinting → Plan Collector → Optimization Engine → Index Advisor → Benchmark Engine → Metrics Store → Grafana

with PostgreSQL/MySQL, pg_stat_monitor/pg_stat_statements, Prometheus, Grafana, HypoPG, and specialized SQL-analysis tooling forming the core.

For a more sophisticated pganalyze/EverSQL-style platform, the architecture can be extended to:

Query Capture → Workload Aggregation → Plan History → Anomaly Detection → Root-Cause Analysis → Optimization Recommendations → What-If Index Testing → Query Rewrite → Benchmark → Approval → Production

This enables teams to build a self-hosted platform that not only monitors database performance but also systematically moves toward automated query optimization.

How to Contribute

Fork the repo.

Add/edit entries in README.md (follow existing format).

Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

Prefer actively maintained projects with a public repository.

Clearly distinguish between fully open-source, source-available, open-core, and commercial hosted offerings.

For database-performance projects, specify whether a project primarily handles query analysis, execution plans, indexing, workload monitoring, database diagnostics, configuration tuning, benchmarking, or observability.

Submit PR with a short explanation.

Star the repo if you find it useful!

Disclaimer

This is a community-curated list — not exhaustive and not an endorsement.

Dedicated open-source end-to-end query-optimization platforms are less common than commercial database-performance products.

Some projects listed here are database extensions, monitoring tools, analyzers, or optimization building blocks rather than direct replacements for enterprise SaaS platforms.

Query optimization recommendations should be validated against representative production workloads before deployment.

EXPLAIN ANALYZE can execute the query being analyzed, so care should be taken with write queries and expensive production workloads.

Open-source deployments require appropriate security, monitoring, backup, access control, and operational practices.

Licensing varies by project. Verify the current license and commercial-use requirements before deployment.

Made for database administrators, backend engineers, SREs, platform engineers, data engineers, database developers, and organizations operating performance-critical SQL workloads.
Let's make database performance optimization more open, observable, automated, and self-hostable.
