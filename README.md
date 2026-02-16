# Awesome Postgres [![awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) ⭐ 437,718 | 🐛 71 | 📅 2026-01-28 with stars

[<img src="https://wiki.postgresql.org/images/a/a4/PostgreSQL_logo.3colors.svg" align="right"  width="100">](https://www.postgresql.org/)

> A curated list of awesome [PostgreSQL](https://www.postgresql.org/) software, libraries, tools and resources, inspired by [awesome-mysql](http://shlomi-noach.github.io/awesome-mysql/)

[PostgreSQL](https://en.wikipedia.org/wiki/PostgreSQL), often simply Postgres, is an [object-relational database](https://en.wikipedia.org/wiki/Object-relational_database) (ORDBMS). PostgreSQL is [ACID-compliant](https://en.wikipedia.org/wiki/ACID) and [transactional](https://en.wikipedia.org/wiki/Transaction_processing). (see more: [wikipedia:PostgreSQL](https://en.wikipedia.org/wiki/PostgreSQL), [PostgreSQL.org](https://www.postgresql.org))

:elephant: Contributions welcome. Add links through [pull requests](https://github.com/dhamaniasad/awesome-postgres/pulls) ⭐ 11,688 | 🐛 17 | 📅 2026-02-14 or create an [issue](https://github.com/dhamaniasad/awesome-postgres/issues) ⭐ 11,688 | 🐛 17 | 📅 2026-02-14 to start a discussion. Please take a look at the [contribution guidelines](origin/CONTRIBUTING.md).

## Contents

* [Awesome Postgres](#awesome-postgres-)
  * [High-Availability](#high-availability)
  * [Backups](#backups)
  * [GUI](#gui)
  * [Distributions](#distributions)
  * [CLI](#cli)
  * [Server](#server)
  * [Monitoring](#monitoring)
  * [Extensions](#extensions)
  * [Platforms](#platforms)
  * [Work Queues](#work-queues)
  * [Optimization](#optimization)
  * [Utilities](#utilities)
  * [Language bindings](#language-bindings)
  * [PaaS (PostgreSQL as a Service)](#paas-postgresql-as-a-service)
  * [Docker images](#docker-images)
  * [Kubernetes](#kubernetes)
* [Resources](#resources)
  * [Tutorials](#tutorials)
  * [Blogs](#blogs)
  * [Documentation](#documentation)
  * [Newsletters](#newsletters)
  * [Videos](#videos)
  * [Community](#community)
  * [Roadmaps](#roadmaps)
  * [External lists](#external-lists)

### High-Availability

* [Patroni](https://github.com/zalando/patroni) ⭐ 8,157 | 🐛 75 | 🌐 Python | 📅 2026-01-29 - Template for PostgreSQL HA with ZooKeeper or etcd.
* [Stolon](https://github.com/sorintlab/stolon) ⭐ 4,807 | 🐛 152 | 🌐 Go | 📅 2024-07-08 - PostgreSQL HA based on Consul or etcd, with Kubernetes integration.
* [autobase](https://github.com/vitabaks/autobase) ⭐ 3,926 | 🐛 36 | 🌐 TypeScript | 📅 2026-02-16 - Autobase for PostgreSQL® is an open-source DBaaS that automates the deployment and management of highly available PostgreSQL clusters.
* [repmgr](https://github.com/2ndQuadrant/repmgr) ⭐ 1,685 | 🐛 129 | 🌐 C | 📅 2025-04-17 - Open-source tool suite to manage replication and failover in a cluster of PostgreSQL servers.
* [pg\_auto\_failover](https://github.com/citusdata/pg_auto_failover) ⭐ 1,325 | 🐛 121 | 🌐 C | 📅 2025-11-17 - Postgres extension and service for automated failover and high-availability.
* [Spock](https://github.com/pgEdge/spock) ⭐ 671 | 🐛 20 | 🌐 C | 📅 2026-02-14 - 100% open-source logical multi-master PostgreSQL replication.
* [BDR](https://github.com/2ndQuadrant/bdr) ⭐ 359 | 🐛 113 | 🌐 C | 📅 2020-02-20 - BiDirectional Replication - a multimaster replication system for PostgreSQL
* [PAF](https://github.com/ClusterLabs/PAF) ⭐ 346 | 🐛 20 | 🌐 Perl | 📅 2024-06-13 - PostgreSQL Automatic Failover: High-Availibility for Postgres, based on Pacemaker and Corosync.
* [SkyTools](https://github.com/pgq/skytools-legacy) ⚠️ Archived - Replication tools, including PgQ, a queuing system, and Londiste, a replication system a bit simpler to manage than Slony.
* [pglookout](https://github.com/aiven/pglookout) ⭐ 189 | 🐛 12 | 🌐 Python | 📅 2025-01-17 - Replication monitoring and failover daemon.
* [pgrwl](https://github.com/hashmap-kz/pgrwl) ⭐ 84 | 🐛 32 | 🌐 Go | 📅 2026-01-19 - Stream write-ahead logs (WAL) from a PostgreSQL server in real time. A drop-in, container-friendly alternative to pg\_receivewal.
* [pg-status](https://github.com/krylosov-aa/pg-status) ⭐ 65 | 🐛 1 | 🌐 C | 📅 2026-02-15 - A microservice that provides HTTP endpoints for instantly retrieving the current master host or a replica that meets various criteria.
* [Slony-I](https://slony.info/) - "Master to multiple slaves" replication system with cascading and failover.

### Backups

* [wal-g](https://github.com/wal-g/wal-g) ⭐ 3,935 | 🐛 336 | 🌐 Go | 📅 2026-02-15 - The successor of WAL-E rewritten in Go. Currently supports cloud object storage services by AWS (S3), Google Cloud (GCS), Azure, as well as OpenStack Swift, MinIO, and file system storages. Supports block-level incremental backups, offloading backup tasks to a standby server, provides parallelization and throttling options. In addition to Postgres, WAL-G can be used for MySQL and MongoDB databases.
* [wal-e](https://github.com/wal-e/wal-e) ⭐ 3,472 | 🐛 93 | 🌐 Python | 📅 2023-12-20 (obsolete) - Simple Continuous Archiving for PostgreSQL to S3, Azure, or Swift by Heroku.
* [pgbackweb](https://github.com/eduardolat/pgbackweb) ⭐ 2,501 | 🐛 92 | 🌐 Go | 📅 2025-11-21 - A Complete Docker-based Postgres backup and maintenance tool with Web UI.
* [pghoard](https://github.com/aiven/pghoard) ⭐ 1,395 | 🐛 55 | 🌐 Python | 📅 2026-02-13 - Backup and restore tool for cloud object stores (AWS S3, Azure, Google Cloud, OpenStack Swift).
* [pg\_probackup](https://github.com/postgrespro/pg_probackup) ⭐ 779 | 🐛 186 | 🌐 Python | 📅 2025-12-09 – A fork of pg\_arman, improved by @PostgresPro, supports incremental backups, backups from replica, multithreaded backup and restore, and anonymous backup without archive command.
* [pg\_back](https://github.com/orgrim/pg_back/) ⭐ 565 | 🐛 9 | 🌐 Go | 📅 2025-12-19 - pg\_back is a simple backup script
* [OmniPITR](https://github.com/omniti-labs/omnipitr) ⭐ 180 | 🐛 3 | 🌐 Perl | 📅 2019-06-25 - Advanced WAL File Management Tools for PostgreSQL.
* [pg-backups-to-s3](https://github.com/Saicheg/pg-backups-to-s3) ⭐ 18 | 🐛 0 | 🌐 PLpgSQL | 📅 2025-05-30 - Docker-first solution on top of pg\_dump with support for environment-based configuration for scheduled PostgreSQL backups with optional compression, GPG encryption, webhooks, automatic upload to Amazon S3.
* [pgbackup-sidecar](https://github.com/Musab520/pgbackup-sidecar) ⭐ 5 | 🐛 0 | 🌐 Shell | 📅 2024-11-08 - `pgbackup-sidecar` is a lightweight Docker sidecar container designed to automate regular backups of a PostgreSQL database using `pg_dump`, `cron`, and bash scripts while also sending output to a webhook.
* [postgres-backup-oss](https://github.com/isaced/postgres-backup-oss) ⭐ 1 | 🐛 0 | 🌐 Shell | 📅 2025-05-12 - A handy Docker container to periodically backup PostgreSQL to Alibaba Cloud Object Storage Service (OSS)
* [Barman](https://www.pgbarman.org/index.html) - Backup and Recovery Manager for PostgreSQL by 2ndQuadrant.
* [Databasus](https://databasus.com) - tool for scheduled PostgreSQL backups via web UI with external storages (local, S3, FTP, Google Drive, etc.), notifications (webhook, Discord, Slack, etc.) and team management.
* [pgBackRest](https://pgbackrest.org/)  - Reliable PostgreSQL Backup & Restore.
* [pitrery](https://dalibo.github.io/pitrery/) - pitrery is a set of Bash scripts to manage Point In Time Recovery (PITR) backups for PostgreSQL.

### GUI

* [Redash](https://github.com/getredash/redash) ⭐ 28,222 | 🐛 739 | 🌐 Python | 📅 2026-02-13 - Connect to any data source, easily visualize and share your data.
* [Teable](https://github.com/teableio/teable) ⭐ 20,872 | 🐛 162 | 🌐 TypeScript | 📅 2026-02-13 - A Super fast, Real-time, Professional, Developer friendly, No code database.
* [pgweb](https://github.com/sosedoff/pgweb) ⭐ 9,256 | 🐛 41 | 🌐 Go | 📅 2026-02-01 - Web-based PostgreSQL database browser written in Go.
* [Postbird](https://github.com/Paxa/postbird) ⭐ 1,619 | 🐛 53 | 🌐 JavaScript | 📅 2025-06-30 - PostgreSQL Client for macOS.
* [PgManage](https://github.com/commandprompt/pgmanage) ⭐ 982 | 🐛 50 | 🌐 PLpgSQL | 📅 2026-02-13 - A modern multi-platform Postgres-centric database client/administration tool.
* [phpPgAdmin](https://github.com/phppgadmin/phppgadmin) ⭐ 840 | 🐛 73 | 🌐 PHP | 📅 2024-07-30 - The Premier Web Based Administration Tool for PostgreSQL.
* [temBoard](https://github.com/dalibo/temboard) ⭐ 753 | 🐛 86 | 🌐 Python | 📅 2025-12-11 - Web-based PostgreSQL GUI and monitoring.
* [Adminer](https://www.adminer.org/) - Full-featured database management tool written in PHP.
* [Beekeeper Studio](https://www.beekeeperstudio.io) - Free and open source SQL client with a modern UI and great Postgres support. Cross platform.
* [Bytebase](https://www.bytebase.com) - Database DevSecOps solution for Developer, Security, DBA, and Platform Engineering teams.
* [Chartbrew](https://chartbrew.com) - Create live dashboards, charts, and client reports from PostgreSQL data. Features a query tool that works with SQL.
* [Count](https://count.co/) - Web-based analytics platform with a notebook interface which connects to PostgreSQL (Commercial Software).
* [DataGrip](https://www.jetbrains.com/datagrip/) - IDE with advanced tool sets and good cross-platform experience (Commercial Software).
* [Datazenit](https://datazenit.com/) - Web-based PostgreSQL GUI (Commercial Software).
* [DataRow](https://www.datarow.com/) - Cross-platform SQL Client for Amazon Redshift: Simple, Effortless, Extensible.
* [DBConvert Streams](https://streams.dbconvert.com/) - A cloud-native platform for real-time data migration and CDC replication between PostgreSQL and MySQL databases across various cloud environments. (Commercial Software).
* [DBeaver](https://dbeaver.io/) - Universal Database Manager with excellent support for PostgreSQL.
* [dbForge Edge](https://www.devart.com/dbforge/edge/) - All-in-one multidatabase solution supporting PostgreSQL, MySQL, MariaDB, SQL Server, Oracle, and a wide range of related cloud services (Commercial Software).
* [DbVisualizer](http://www.dbvis.com) - Cross-platform database client for developers, DBAs, and analysts (Commercial Software).
* [Holistics](https://www.holistics.io/) - Online cross platform database management tool and SQL query reporting GUI with strong PostgreSQL support (Commercial Software).
* [JackDB](https://www.jackdb.com/) - Web-based SQL query interface (Commercial Software).
* [Luna Modeler](http://www.datensen.com) - Cross-platform desktop data modeling tool (Commercial Software).
* [Mathesar](https://mathesar.org/) -  Web application providing an intuitive user experience to databases.
* [Metabase](https://www.metabase.com/) - Simple dashboards, charts and query tool for PostgreSQL.
* [Numeracy](https://numeracy.co/) - Fast SQL editor with charts and dashboards for PostgreSQL (Commercial Software).
* [pgAdmin](https://www.pgadmin.org/) - PostgreSQL Administration and Management GUI.
* [pgMagic🪄](https://pgmagic.app/?ref=awesomepostgres) - Chat to Postgres in Natural Language (Commercial Software).
* [pgModeler](https://pgmodeler.io/) - pgModeler is an open-source PostgreSQL Database Modeler.
* [PostgresCompare](https://www.postgrescompare.com) - Cross-platform database comparison and deployment tool (Commercial Software).
* [Postico](https://eggerapps.at/postico/) - Modern PostgreSQL Client for macOS (Commercial Software).
* [PSequel](http://www.psequel.com/) - Clean and simple interface to perform common PostgreSQL tasks quickly (Commercial Software).
* [SQL Tabs](http://www.sqltabs.com/) - Cross Platform Desktop Client for PostgreSQL written in JS.
* [SQLPro for Postgres](http://macpostgresclient.com/) - Simple, powerful PostgreSQL manager for macOS (Commercial Software).
* [TablePlus](https://tableplus.com/) - Native App which let you edit database and structure. High-end security ensured (Commercial Software).
* [Valentina Studio](https://www.valentina-db.com/en/valentina-studio-overview) - Cross-platform database administration tool (Free/Commercial)
* [DbGate](https://dbgate.org) - The Smartest (no)SQL Database Client
* [WebDB](https://webdb.app) – Efficient Database IDE.

### Distributions

* [Postgres.app](https://postgresapp.com/) - The Easiest Way to Get Started with PostgreSQL on macOS.
* [Pigsty](https://github.com/Vonng/pigsty) ⭐ 4,683 | 🐛 16 | 🌐 Shell | 📅 2026-02-13 - Battery-Included Open-Source Distribution for PostgreSQL with ultimate observability & Database-as-Code toolbox for developers.

### CLI

* [pgcli](https://github.com/dbcli/pgcli) ⭐ 13,023 | 🐛 59 | 🌐 Python | 📅 2026-01-17 - Postgres CLI with autocompletion and syntax highlighting
* [atlas](https://github.com/ariga/atlas) ⭐ 8,083 | 🐛 241 | 🌐 Go | 📅 2026-02-07 - Atlas is a tool for managing and migrating database schemas using modern DevOps principles.
* [schemaspy](https://github.com/schemaspy/schemaspy) ⭐ 3,537 | 🐛 297 | 🌐 HTML | 📅 2026-01-26 - SchemaSpy is a JAVA JDBC-compliant tool for generating your database to HTML documentation, including Entity Relationship diagrams
* [pg-schema-diff](https://github.com/stripe/pg-schema-diff) ⭐ 797 | 🐛 57 | 🌐 Go | 📅 2026-01-07 - CLI (and Golang library) for diffing Postgres schemas and generating SQL migrations with minimal locking.
* [pgsh](https://github.com/sastraxi/pgsh) ⭐ 597 | 🐛 34 | 🌐 JavaScript | 📅 2023-01-11 - Branch your PostgreSQL Database like Git
* [psql2csv](https://github.com/fphilipe/psql2csv) ⭐ 186 | 🐛 2 | 🌐 Shell | 📅 2022-02-23 - Run a query in psql and output the result as CSV
* [pgschema](https://www.pgschema.com) - Terraform-style declarative schema migration for Postgres
* [psql](https://www.postgresql.org/docs/current/static/app-psql.html) - The built-in PostgreSQL CLI client
* [pdot](https://gitlab.com/dmfay/pdot) - Visualize and explore database structures in your shell, from high-context views of the foreign key graph to trigger cascades, role inheritance and permissions, and many more

### Server

* [AgensGraph](https://bitnine.net/) - Powerful graph database based on the PostgreSQL.
* [Apache Cloudberry](https://github.com/apache/cloudberry) ⭐ 1,187 | 🐛 165 | 🌐 C | 📅 2026-02-16 - And MPP PostgreSQL fork. Open source alternative to Greenplum Database.
* [FerretDB](https://www.ferretdb.io) - A truly Open Source MongoDB alternative on top of PostgreSQL.
* [Postgres-XL](https://www.postgres-xl.org/) - Scalable Open Source PostgreSQL-based Database Cluster.
* [YugabyteDB](https://yugabyte.com/) - Open Source Distributed SQL using  a fork of PostgreSQL on top of distributed storage and transaction

### Security

* [Acra](https://github.com/cossacklabs/acra) ⭐ 1,453 | 🐛 16 | 🌐 Go | 📅 2025-12-05 - SQL database security suite: proxy for data protection with transparent "on the fly" data encryption, SQL firewall (SQL injections prevention), intrusion detection system.

### Monitoring

* [coroot](https://github.com/coroot/coroot) ⭐ 7,387 | 🐛 118 | 🌐 Go | 📅 2026-02-12 - Coroot is an open-source APM & Observability tool, a DataDog and NewRelic alternative. Powered by eBPF for rapid insights into system performance.
* [postgres\_exporter](https://github.com/wrouesnel/postgres_exporter) ⭐ 3,410 | 🐛 344 | 🌐 Go | 📅 2026-02-11 - Prometheus exporter for PostgreSQL server metrics.
* [dexter](https://github.com/ankane/dexter) ⭐ 2,062 | 🐛 2 | 🌐 Ruby | 📅 2025-12-26 - The automatic indexer for Postgres. Detects slow queries and creates indexes if configured to do so.
* [pgwatch2](https://github.com/cybertec-postgresql/pgwatch2) ⚠️ Archived - Flexible and easy to get started PostgreSQL metrics monitor focusing on Grafana dashboards.
* [Pome](https://github.com/rach/pome) ⭐ 1,077 | 🐛 15 | 🌐 Go | 📅 2020-09-04 - Pome stands for PostgreSQL Metrics. Pome is a PostgreSQL Metrics Dashboard to keep track of the health of your database.
* [PMM](https://github.com/percona/pmm) ⭐ 965 | 🐛 171 | 🌐 Go | 📅 2026-02-16 - Percona Monitoring and Management (PMM) is a Free and Open Source platform for monitoring and managing PostgreSQL, MySQL, and MongoDB.
* [Check\_postgres](https://github.com/bucardo/check_postgres) ⭐ 593 | 🐛 101 | 🌐 Perl | 📅 2025-01-02 - Nagios check\_postgres plugin for checking status of PostgreSQL databases.
* [pg\_view](https://github.com/zalando/pg_view) ⭐ 505 | 🐛 28 | 🌐 Python | 📅 2023-03-25 - Open-source command-line tool that shows global system stats, per-partition information, memory stats and other information.
* [pg\_exporter](https://github.com/Vonng/pg_exporter) ⭐ 299 | 🐛 13 | 🌐 Go | 📅 2026-02-12 - Fully customizable Prometheus exporter for PostgreSQL & Pgbouncer with fine-grained execution control.
* [check\_pgactivity](https://github.com/OPMDG/check_pgactivity) ⭐ 180 | 🐛 49 | 🌐 Perl | 📅 2026-02-09 - check\_pgactivity is designed to monitor PostgreSQL clusters from Nagios. It offers many options to measure and monitor useful performance metrics.
* [libzbxpgsql](https://github.com/cavaliercoder/libzbxpgsql) ⭐ 155 | 🐛 51 | 🌐 C | 📅 2023-11-14 - Comprehensive PostgreSQL monitoring module for Zabbix.
* [Instrumental](https://github.com/Instrumental/instrumentald) ⭐ 15 | 🐛 8 | 🌐 HTML | 📅 2018-09-17 - Real-time performance monitoring, including [pre-made graphs](https://instrumentalapp.com/docs/instrumentald/postgresql#suggested-graphs) for ease of setup (Commercial Software)
* [Datadog](https://www.datadoghq.com/product/database-monitoring/) - SaaS monitoring that collects and visualizes metrics, queries, and explain plans, and sends alerts when problems are encountered (Commercial Software).
* [pgmetrics](https://pgmetrics.io/) - pgmetrics is an open-source, zero-dependency, single-binary tool that can collect a lot of information and statistics from a running PostgreSQL server and display it in easy-to-read text format or export it as JSON and CSV for scripting.
* [pgbench](https://www.postgresql.org/docs/devel/static/pgbench.html) - Run a benchmark test on PostgreSQL.
* [opm.io](http://opm.io) -  Open PostgreSQL Monitoring is a free software suite designed to help you manage your PostgreSQL servers. It can gather stats, display dashboards and send warnings when something goes wrong.
* [okmeter.io](https://okmeter.io/pg) - Commercial SaaS agent-based monitoring with a very detailed PostgreSQL plugin. It automatically gathers 100s of stats, displays dashboards on every aspect and sends alerts when something goes wrong (Commercial Software).
* [StatsMgr](https://codeberg.org/data-bene/statsmgr) - An open-source PostgreSQL extension designed for efficient and organized advanced statistics management.

### Extensions

* [Citus](https://github.com/citusdata/citus) ⭐ 12,289 | 🐛 1,050 | 🌐 C | 📅 2026-02-13 - Scalable PostgreSQL cluster for real-time workloads.
* [pg\_search](https://github.com/paradedb/paradedb) ⭐ 8,338 | 🐛 115 | 🌐 Rust | 📅 2026-02-16 - pg\_search is a PostgreSQL extension that enables full-text search over SQL tables using the BM25 algorithm, the state-of-the-art ranking function for full-text search.
* [ParadeDB](https://github.com/paradedb/paradedb) ⭐ 8,338 | 🐛 115 | 🌐 Rust | 📅 2026-02-16 -  Postgres for Search and Analytics
* [zomboDB](https://github.com/zombodb/zombodb) ⚠️ Archived - Extension that enables efficient full-text searching via the use of indexes backed by Elasticsearch.
* [AGE](https://github.com/apache/age) ⭐ 4,226 | 🐛 178 | 🌐 C | 📅 2026-02-14 - Adds fully-functional graph database support including Cypher queries.
* [pg\_cron](https://github.com/citusdata/pg_cron) ⭐ 3,661 | 🐛 129 | 🌐 C | 📅 2025-12-22 - Run periodic jobs in PostgreSQL.
* [pg\_partman](https://github.com/pgpartman/pg_partman) ⭐ 2,597 | 🐛 53 | 🌐 PLpgSQL | 📅 2026-02-16 - Partition management extension for PostgreSQL.
* [cstore\_fdw](https://github.com/citusdata/cstore_fdw) ⭐ 1,786 | 🐛 69 | 🌐 C | 📅 2021-03-08 - Columnar store for analytics with PostgreSQL.
* [HypoPG](https://github.com/HypoPG/hypopg) ⭐ 1,606 | 🐛 4 | 🌐 C | 📅 2026-02-08 - HypoPG provides hypothetical/virtual indexes feature.
* [pgRouting](https://github.com/pgRouting/pgrouting) ⭐ 1,369 | 🐛 73 | 🌐 C++ | 📅 2026-02-07 - pgRouting extends the PostGIS/PostgreSQL geospatial database to provide geospatial routing and other network analysis functionality.
* [pglogical](https://github.com/2ndQuadrant/pglogical) ⭐ 1,199 | 🐛 186 | 🌐 C | 📅 2026-02-15 - Extension that provides logical streaming replication.
* [pg\_shard](https://github.com/citusdata/pg_shard) ⭐ 1,062 | 🐛 38 | 🌐 C | 📅 2016-08-03 - Extension to scale out real-time reads and writes.
* [plpgsql\_check](https://github.com/okbob/plpgsql_check) ⭐ 738 | 🐛 4 | 🌐 C | 📅 2026-02-15 - Extension that allows to check plpgsql source code.
* [pg\_squeeze](https://github.com/cybertec-postgresql/pg_squeeze) ⭐ 647 | 🐛 2 | 🌐 C | 📅 2025-10-08 - An extension for automatic bloat cleanup with minimal locking.
* [pg\_stat\_monitor](https://github.com/percona/pg_stat_monitor) ⭐ 557 | 🐛 8 | 🌐 Perl | 📅 2026-02-13 - Query Performance Monitoring tool for PostgreSQL.
* [pgMemento](https://github.com/pgMemento/pgMemento) ⭐ 400 | 🐛 12 | 🌐 PLpgSQL | 📅 2025-03-11 - Provides an audit trail for your data inside a PostgreSQL database using triggers and server-side functions written in PL/pgSQL.
* [pgcat](https://github.com/kingluo/pgcat) ⭐ 386 | 🐛 1 | 🌐 Go | 📅 2024-09-26 - Enhanced PostgreSQL logical replication
* [pg\_paxos](https://github.com/citusdata/pg_paxos/) ⚠️ Archived - Basic implementation of Paxos and Paxos-based table replication for a cluster of PostgreSQL nodes.
* [PG\_Themis](https://github.com/cossacklabs/pg_themis) ⭐ 33 | 🐛 1 | 🌐 C | 📅 2016-12-12 - Postgres binding as extension for crypto library Themis, providing various security services on PgSQL's side.
* [pg\_barcode](https://github.com/btouchard/pg_barcode/) ⭐ 1 | 🐛 0 | 🌐 C | 📅 2025-01-09 - PostgreSQL SVG QRcode & Datamatrix generator.
* [pgxn](https://pgxn.org/) PostgreSQL Extension Network - central distribution point for many open-source PostgreSQL extensions.
* [Extensions listing by joelonsql](https://gist.github.com/joelonsql/e5aa27f8cc9bd22b8999b7de8aee9d47) - 1000+ PostgreSQL extensions.
* [Pigsty extensions catalogue](https://ext.pigsty.io/list/) - 400+ PostgreSQL extensions.
* [OrioleDB](https://www.orioledb.com/) - The cloud-native storage engine for PostgreSQL. OrioleDB is a PostgreSQL extension that combines the advantages of both on-disk and in-memory engines.
* [cyanaudit](https://pgxn.org/dist/cyanaudit/) - Cyan Audit provides in-database logging of all DML activity on a column-by-column basis.
* [PGStrom](https://wiki.postgresql.org/wiki/PGStrom) - Extension to offload CPU intensive workloads to GPU.
* [PipelineDB](https://www.confluent.io/blog/pipelinedb-team-joins-confluent/) - A PostgreSQL extension that runs SQL queries continuously on streams, incrementally storing results in tables.
* [PostGIS](http://postgis.net/) - Spatial and Geographic objects for PostgreSQL.
* [TimescaleDB](https://www.timescale.com/) - Open-source time-series database fully compatible with Postgres, distributed as extension
* [pgTAP](https://pgtap.org/) - Database testing framework for Postgres
* [PGroonga](https://pgroonga.github.io/) - PGroonga provides a new index access method that uses Groonga allowing super fast full text search feature against all languages.
* [PGAudit](https://www.pgaudit.org/) - The PostgreSQL Audit Extension (or pgaudit) provides detailed session and/or object audit logging via the standard logging facility provided by PostgreSQL.
* [PostgresML](https://postgresml.org/) - Machine learning and AI inside your database, including vectors, LLMs, and classic ML. Train, predict and manage the entire lifecycle of machine learning models using only SQL.
* [PostgreSQL Anonymizer](https://postgresql-anonymizer.readthedocs.io/en/stable/) - An extension to mask or replace personally identifiable information (PII) or commercially sensitive data from a Postgres database, through PG Security Labels.

### Platforms

* [Atlas4D](https://github.com/crisbez/atlas4d-base) ⭐ 7 | 🐛 8 | 🌐 HTML | 📅 2025-12-25 - Open-source 4D spatiotemporal platform combining PostGIS, TimescaleDB, pgvector, and H3 for unified geospatial and time-series intelligence.

### Work Queues

* [river](https://github.com/riverqueue/river) ⭐ 4,819 | 🐛 41 | 🌐 Go | 📅 2026-02-15 - A high-performance job processing system for Go and Postgres.
* [pgmq](https://github.com/pgmq/pgmq) ⭐ 4,528 | 🐛 44 | 🌐 PLpgSQL | 📅 2026-02-14 - A lightweight message queue. Like AWS SQS and RSMQ but on Postgres.
* [pgBoss](https://github.com/timgit/pg-boss) ⭐ 3,200 | 🐛 31 | 🌐 TypeScript | 📅 2026-02-16 - Queueing jobs in Postgres from Node.js like a boss.
* [BeanQueue](https://github.com/LaunchPlatform/bq) ⭐ 24 | 🐛 3 | 🌐 Python | 📅 2025-08-09 - A Python work queue framework based on SKIP LOCKED, LISTEN and NOTIFY
* [dbos](https://www.dbos.dev/) - Durable workflows in Typescript and Python
* [Graphile Worker](https://worker.graphile.org) - A high performance job queue for PostgreSQL, written in Node.js
* [@andyrmitchell/pg-queue](https://www.npmjs.com/package/@andyrmitchell/pg-queue) - The 'No Maintenance' Postgres Queue for Node.js

### Optimization

* [PgHero](https://github.com/ankane/pghero) ⭐ 8,790 | 🐛 15 | 🌐 Ruby | 📅 2025-12-26 - PostgreSQL insights made easy.
* [PEV2](https://github.com/dalibo/pev2) ⭐ 3,356 | 🐛 71 | 🌐 TypeScript | 📅 2026-02-02 - Online Postgres Explain Visualizer.
* [pgtune](https://github.com/le0pard/pgtune) ⭐ 2,653 | 🐛 1 | 🌐 JavaScript | 📅 2026-01-27 - Online version of PostgreSQL configuration wizard.
* [pg\_flame](https://github.com/mgartner/pg_flame) ⭐ 1,614 | 🐛 2 | 🌐 Go | 📅 2020-01-13 - A flamegraph generator for query plans.
* [pgtune](https://github.com/gregs1104/pgtune/) ⭐ 1,081 | 🐛 12 | 🌐 Python | 📅 2021-08-17 - PostgreSQL configuration wizard.
* [TimescaleDB Tune](https://github.com/timescale/timescaledb-tune) ⭐ 490 | 🐛 17 | 🌐 Go | 📅 2025-12-23 - a program for tuning a TimescaleDB database to perform its best based on the host's resources such as memory and number of CPUs.
* [aqo](https://github.com/postgrespro/aqo) ⭐ 478 | 🐛 9 | 🌐 C | 📅 2026-01-20 - Adaptive query optimization for PostgreSQL.
* [pg\_web\_stats](https://github.com/kirs/pg_web_stats) ⭐ 97 | 🐛 3 | 🌐 Ruby | 📅 2018-10-14 - Web UI to view pg\_stat\_statements.
* [pgconfig.org](https://github.com/sebastianwebber/pgconfig) ⚠️ Archived - PostgreSQL Online Configuration Tool (also based on pgtune).
* [pgassistant](https://github.com/beh74/pgassistant-community) ⭐ 24 | 🐛 0 | 🌐 CSS | 📅 2026-02-08 - A PostgreSQL tool for developers to help understand, optimize database with LLM and pgTune integration.
* [EverSQL](https://www.eversql.com/) - Automated query optimization tool, monitoring and analysis tool, indexing recommendation tool. (Commercial Software)
* [pgMustard](https://www.pgmustard.com/) - A modern user interface
  for `EXPLAIN`, that also provides performance tips (Commercial Software).
* [PoWA](https://powa.readthedocs.io/en/latest/) - PostgreSQL Workload Analyzer gathers performance stats and provides real-time charts and graphs to help monitor and tune your PostgreSQL servers.
* [Metis](https://www.metisdata.io/product/troubleshooting) - Metis provides observability and performance tuning for SQL databases including PostgreSQL. (Commercial Software)

### Utilities

* [Hasura GraphQL Engine](https://github.com/hasura/graphql-engine) ⭐ 31,899 | 🐛 2,375 | 🌐 TypeScript | 📅 2026-02-12 - Blazing fast, instant realtime GraphQL APIs on Postgres with fine grained access control, also trigger webhooks on database events.
* [PostgREST](https://github.com/PostgREST/postgrest) ⭐ 26,517 | 🐛 381 | 🌐 Haskell | 📅 2026-02-15 - Serves a fully RESTful API from any existing PostgreSQL database.
* [PostGraphile](https://github.com/graphile/postgraphile) ⭐ 12,901 | 🐛 142 | 🌐 TypeScript | 📅 2026-02-13 - Instant GraphQL API or GraphQL schema for your PostgreSQL database
* [pgloader](https://github.com/dimitri/pgloader) ⭐ 6,287 | 🐛 463 | 🌐 Common Lisp | 📅 2025-06-04 - Loads data into PostgreSQL using the COPY streaming protocol, and does so with separate threads for reading and writing data.
* [pgroll](https://github.com/xataio/pgroll) ⭐ 6,277 | 🐛 91 | 🌐 Go | 📅 2026-02-03 - Zero-downtime, reversible, schema migrations for Postgres
* [pREST](https://github.com/prest/prest) ⭐ 4,519 | 🐛 147 | 🌐 Go | 📅 2026-02-11 - Serve a RESTful API from any PostgreSQL database (Golang)
* [pgbadger](https://github.com/darold/pgbadger) ⭐ 3,944 | 🐛 16 | 🌐 Perl | 📅 2026-02-05 - Fast PostgreSQL Log Analyzer.
* [pgsync](https://github.com/ankane/pgsync) ⭐ 3,429 | 🐛 14 | 🌐 Ruby | 📅 2025-12-26 - Tool to sync PostgreSQL data to your local machine.
* [sqitch](https://github.com/sqitchers/sqitch) ⭐ 3,101 | 🐛 77 | 🌐 Perl | 📅 2026-01-25 - Tool for managing versioned schema deployment
* [migra](https://github.com/djrobstep/migra) ⭐ 3,052 | 🐛 86 | 🌐 Python | 📅 2025-08-25 - Like diff but for Postgres schemas.
* [pg\_activity](https://github.com/dalibo/pg_activity) ⭐ 2,994 | 🐛 13 | 🌐 Python | 📅 2026-01-13 - top like application for PostgreSQL server activity monitoring.
* [sqlcheck](https://github.com/jarulraj/sqlcheck) ⭐ 2,521 | 🐛 13 | 🌐 C++ | 📅 2024-02-21 - Automatically detects common SQL anti-patterns. Such anti-patterns often slow down queries. Addressing them will, therefore, help accelerate queries.
* [pgCenter](https://github.com/lesovsky/pgcenter) ⭐ 1,591 | 🐛 13 | 🌐 Go | 📅 2026-01-06 - Provides convenient interface to various statistics, management task, reloading services, viewing log files and canceling or terminating database backends.
* [ERAlchemy](https://github.com/Alexis-benoist/eralchemy) ⭐ 1,398 | 🐛 10 | 🌐 Python | 📅 2026-01-12 - ERAlchemy generates Entity Relation (ER) diagram from databases.
* [pgfutter](https://github.com/lukasmartinelli/pgfutter) ⭐ 1,344 | 🐛 55 | 🌐 Go | 📅 2020-09-02 - Import CSV and JSON into PostgreSQL the easy way.
* [yoke](https://github.com/nanopack/yoke) ⚠️ Archived - PostgreSQL high-availability cluster with auto-failover and automated cluster recovery.
* [pg\_timetable](https://github.com/cybertec-postgresql/pg_timetable) ⭐ 1,318 | 🐛 2 | 🌐 Go | 📅 2026-02-13 - Advanced job scheduler for PostgreSQL.
* [mysql-postgresql-converter](https://github.com/lanyrd/mysql-postgresql-converter) ⭐ 1,308 | 🐛 29 | 🌐 Python | 📅 2022-09-16 - Lanyrd's MySQL to PostgreSQL conversion script.
* [pgMonitor](https://github.com/CrunchyData/pgmonitor) ⭐ 696 | 🐛 14 | 🌐 PLpgSQL | 📅 2026-02-13 - Postgres metrics collection and visualization that can be deployed to bare metal, virtual machines, or Kubernetes.
* [pgmigrate](https://github.com/yandex/pgmigrate) ⭐ 662 | 🐛 0 | 🌐 Python | 📅 2026-01-07 - CLI tool to evolve schema migrations, developed by Yandex.
* [postgresql-metrics](https://github.com/spotify/postgresql-metrics) ⭐ 598 | 🐛 3 | 🌐 Python | 📅 2023-05-29 - Tool that extracts and provides metrics for your PostgreSQL database.
* [ZSON](https://github.com/postgrespro/zson) ⭐ 563 | 🐛 0 | 🌐 C | 📅 2023-04-14 - PostgreSQL extension for transparent JSONB compression
* [planter](https://github.com/achiku/planter) ⭐ 558 | 🐛 5 | 🌐 Go | 📅 2024-03-30 - Generate PlantUML ER diagram textual description from PostgreSQL tables
* [pg\_chameleon](https://github.com/the4thdoctor/pg_chameleon) ⭐ 429 | 🐛 45 | 🌐 Python | 📅 2025-01-21 - Real time replica from MySQL to PostgreSQL with optional type override migration and migration capabilities.
* [Pyrseas](https://github.com/perseas/Pyrseas) ⭐ 406 | 🐛 47 | 🌐 Python | 📅 2024-07-10 - Postgres database schema versioning.
* [pgclimb](https://github.com/lukasmartinelli/pgclimb) ⭐ 390 | 🐛 15 | 🌐 Go | 📅 2020-06-18 - Export data from PostgreSQL into different data formats.
* [bemi](https://github.com/BemiHQ/bemi) ⭐ 388 | 🐛 0 | 🌐 TypeScript | 📅 2025-12-23 - Automatic data change tracking for PostgreSQL
* [RegreSQL](https://github.com/dimitri/regresql) ⭐ 348 | 🐛 4 | 🌐 Go | 📅 2024-09-04 - Tool to build, maintain and execute a regression testing suite for SQL queries.
* [pg\_insights](https://github.com/lob/pg_insights) ⚠️ Archived - Convenient SQL for monitoring Postgres database health.
* [GatewayD](https://github.com/gatewayd-io/gatewayd) ⭐ 275 | 🐛 87 | 🌐 Go | 📅 2026-02-11 - Cloud-native database gateway and framework for building data-driven applications. Like API gateways, for databases.
* [ldap2pg](https://github.com/dalibo/ldap2pg) ⭐ 230 | 🐛 13 | 🌐 Go | 📅 2025-10-01 - Synchronize roles and privileges from YML and LDAP.
* [PGXN client](https://github.com/pgxn/pgxnclient) ⭐ 158 | 🐛 6 | 🌐 Python | 📅 2024-06-14 - Command line tool to interact with the PostgreSQL Extension Network
* [pgspot](https://github.com/timescale/pgspot) ⭐ 126 | 🐛 5 | 🌐 Python | 📅 2026-02-11 - Spot vulnerabilities in PostgreSQL extension scripts.
* [pg-formatter](https://github.com/gajus/pg-formatter) ⭐ 83 | 🐛 8 | 🌐 TypeScript | 📅 2026-01-21 - A PostgreSQL SQL syntax beautifier (Node.js).
* [pg-spot-operator](https://github.com/pg-spot-ops/pg-spot-operator) ⭐ 59 | 🐛 18 | 🌐 Python | 📅 2026-01-17 - A daemon to run stateful Postgres on cheap AWS Spot VMs
* [NServiceBus.Transport.PostgreSql](https://github.com/Particular/NServiceBus.SqlServer) ⭐ 46 | 🐛 31 | 🌐 C# | 📅 2026-02-10 - The NServiceBus.Transport.PostgreSql library allows .NET developers to [use a PostgreSQL database as a message broker](https://docs.particular.net/transports/postgresql). (Commerical Software)
* [pgcmp](https://github.com/cbbrowne/pgcmp) ⭐ 46 | 🐛 0 | 🌐 Shell | 📅 2024-05-15 - Tool to compare database schemas, with capability to accept some persistent differences
* [pg-differ](https://github.com/multum/pg-differ) ⭐ 40 | 🐛 8 | 🌐 JavaScript | 📅 2021-04-29 - Tool for easy initialization / updating of the structure of PostgreSQL tables, migration alternative (Node.js).
* [pg\_migrate](https://github.com/jwdeitch/pg_migrate) ⭐ 32 | 🐛 0 | 🌐 C | 📅 2017-10-11 - Manage PostgreSQL codebases and make VCS simple.
* [pglistend](https://github.com/kabirbaidhya/pglistend) ⭐ 30 | 🐛 0 | 🌐 JavaScript | 📅 2017-03-29 - A lightweight PostgresSQL `LISTEN`/`NOTIFY` daemon built on top of `node-postgres`.
* [pg\_docs\_bot](https://github.com/mchristofides/pg_docs_bot/) ⭐ 18 | 🐛 0 | 🌐 JavaScript | 📅 2025-04-04 - Browser extension to redirect PostgreSQL docs links to the current version.
* [apgdiff](https://www.apgdiff.com/) - Compares two database dump files and creates output with DDL statements that can be used to update old database schema to new one.
* [flyway](https://flywaydb.org/) - Schema migration tool for Postgres and others.
* [ora2pg](http://ora2pg.darold.net) - Perl module to export an Oracle database schema to a PostgreSQL compatible schema.
* [pganalyze](https://pganalyze.com) - PostgreSQL Performance Monitoring (Commercial Software).
* [PgBouncer](http://www.pgbouncer.org/) - Lightweight connection pooler for PostgreSQL.
* [PGInsight](http://pginsight.io/) - CLI tool to easily dig deep inside your PostgreSQL database.
* [pgpool-II](https://www.pgpool.net/mediawiki/index.php/Main_Page) - Middleware that provides connection pooling, replication, load balancing and limiting exceeding connections.
* [pg\_bulkload](http://ossc-db.github.io/pg_bulkload/index.html) - It's a high speed data loading utility for PostgreSQL.
* [postgres-checkup](https://gitlab.com/postgres-ai/postgres-checkup) - a new-generation diagnostics tool that allows users to collect deep analysis of the health of a Postgres database.
* [ScaffoldHub.io](https://scaffoldhub.io) - Generate fullstack PostgreSQL apps with Angular, Vue or React (Commercial Software).

### Language bindings

* Node: [node-postgres](https://github.com/brianc/node-postgres) ⭐ 13,064 | 🐛 498 | 🌐 JavaScript | 📅 2026-02-13, [pg-promise](https://github.com/vitaly-t/pg-promise) ⭐ 3,549 | 🐛 0 | 🌐 JavaScript | 📅 2026-02-11, [pogi](https://github.com/holdfenytolvaj/pogi) ⭐ 139 | 🐛 7 | 🌐 TypeScript | 📅 2026-02-04, [slonik](https://github.com/gajus/slonik) ⭐ 4,886 | 🐛 29 | 🌐 TypeScript | 📅 2026-02-12, [postgres](https://github.com/porsager/postgres) ⭐ 8,551 | 🐛 250 | 🌐 JavaScript | 📅 2026-01-06
* Go: [pq](https://github.com/lib/pq) ⭐ 9,793 | 🐛 84 | 🌐 Go | 📅 2026-02-12, [pgx](https://github.com/jackc/pgx) ⭐ 13,330 | 🐛 252 | 🌐 Go | 📅 2026-02-15, [go-pg](https://github.com/go-pg/pg) ⭐ 5,787 | 🐛 121 | 🌐 Go | 📅 2025-11-26
* Rust: [rust-postgresql](https://github.com/sfackler/rust-postgres) ⭐ 3,903 | 🐛 148 | 🌐 Rust | 📅 2026-02-03, [pgx](https://github.com/tcdi/pgx) ⭐ 4,363 | 🐛 333 | 🌐 Rust | 📅 2026-02-09, [wtx](https://github.com/c410-f3r/wtx) ⭐ 342 | 🐛 12 | 🌐 Rust | 📅 2026-02-11
* .Net/.Net Core: [Npgsql](https://github.com/npgsql/npgsql) ⭐ 3,653 | 🐛 234 | 🌐 C# | 📅 2026-02-11
* TypeScript: [zapatos](https://github.com/jawj/zapatos) ⭐ 1,397 | 🐛 51 | 🌐 TypeScript | 📅 2025-09-19
* Elixir: [postgrex](https://github.com/elixir-ecto/postgrex) ⭐ 1,199 | 🐛 6 | 🌐 Elixir | 📅 2026-02-01
* Ruby: [pg](https://github.com/ged/ruby-pg) ⭐ 854 | 🐛 16 | 🌐 C | 📅 2026-02-12
* Zig: [pg.zig](https://github.com/karlseguin/pg.zig) ⭐ 487 | 🐛 4 | 🌐 Zig | 📅 2026-02-15
* Common Lisp: [Postmodern](https://github.com/marijnh/Postmodern) ⭐ 426 | 🐛 5 | 🌐 Common Lisp | 📅 2025-07-24
* R: [RPostgres](https://github.com/r-dbi/RPostgres) ⭐ 337 | 🐛 30 | 🌐 R | 📅 2026-02-16, [RPostgreSQL](https://github.com/tomoakin/RPostgreSQL) ⭐ 66 | 🐛 48 | 🌐 C | 📅 2025-03-28
* Clojure: [clj-postgresql](https://github.com/remodoy/clj-postgresql) ⭐ 162 | 🐛 9 | 🌐 Clojure | 📅 2025-03-07
* Lua: [luapgsql](https://github.com/arcapos/luapgsql) ⭐ 117 | 🐛 7 | 🌐 C | 📅 2026-02-07
* PHP: [Pomm](http://www.pomm-project.org), [pecl/pq](https://github.com/m6w6/ext-pq) ⭐ 41 | 🐛 3 | 🌐 C | 📅 2025-09-04
* Haskell: [postgresql-simple](http://hackage.haskell.org/package/postgresql-simple)
* Java: [PostgreSQL JDBC Driver](https://jdbc.postgresql.org/), [Vert.x PostgreSQL Client](https://vertx.io/docs/vertx-pg-client/java/)
* Perl: [DBD-Pg](https://metacpan.org/pod/distribution/DBD-Pg/Pg.pm)
* Python: [psycopg2](https://pypi.org/project/psycopg2/), [asyncpg](https://pypi.org/project/asyncpg/), [pg8000](https://pypi.org/project/pg8000/)

### PaaS *(PostgreSQL as a Service)*

* [Aiven PostgreSQL](https://aiven.io/postgresql) - PostgreSQL as a service in AWS, Azure, DigitalOcean, Google Cloud and UpCloud; plans range from $19/month single node instances to large highly-available setups, free trial for two weeks.
* [Amazon RDS for PostgreSQL](https://aws.amazon.com/rds/postgresql/) - Amazon Relational Database Service (RDS) for PostgreSQL
* [Azure Database for PostgreSQL](https://azure.microsoft.com/en-us/services/postgresql/) - Azure Database for PostgreSQL provides fully managed, enterprise-ready community PostgreSQL database as a service. It provides builtin HA, elastic scaling and native integration with Azure ecosystem.
* [Crunchy Bridge](https://www.crunchydata.com/products/crunchy-bridge/) - Fully managed Postgres from the Postgres experts. Available across all major cloud providers: Amazon AWS, Google GCP, Microsoft Azure. No lock-in with full super-user support.
* [Database Labs](https://www.databaselabs.io) - Get a production-ready cloud PostgreSQL server in minutes, from $20 a month Backups, monitoring, patches, and 24/7 tech support all included.
* [DigitalOcean Managed Databases](https://www.digitalocean.com/products/managed-databases/) - Fully managed PostgreSQL databases. No free plan. Starting at $15/mo. Daily backups with point-in-time recovery. Standby nodes with auto-failover.
* [Google Cloud SQL for PostgreSQL](https://cloud.google.com/sql/docs/postgres/) - Fully-managed database service that makes it easy to set up, maintain, manage, and administer your PostgreSQL relational databases on Google Cloud Platform.
* [Heroku Postgres](https://elements.heroku.com/addons/heroku-postgresql) - Plans from free to huge, operated by PostgreSQL experts. Does not require running your app on Heroku. Free plan includes 10,000 rows, 20 connections, up to two backups, and has PostGIS support.
* [OVHcloud Cloud Databases](https://www.ovhcloud.com/en/public-cloud/databases/) - Highly available, scalable, and secured PostgreSQL. Daily backups with point-in-time recovery, no lock-in, free incoming and outgoing traffic.
* [Render Managed PostgreSQL](https://render.com/docs/databases) - Secure, reliable, and completely hands-off managed PostgreSQL. Encryption at rest, automated backups, and expandable SSD storage included in all plans. Plans start at $7 per month for 256MB RAM and 1GB storage (free for first 90 days).
* [ScaleGrid PostgreSQL DBaaS](https://scalegrid.io/postgresql.html) - Fully managed PostgreSQL hosting with high availability, dedicated servers, and superuser control on the #1 multi-cloud Amazon RDS alternative.
* [Scaleway Managed Database](https://www.scaleway.com/en/database/) - Fully managed PostgreSQL databases with HA, scaling, and automated backups, hosted in the EU. Starting at €10 per month.
* [Supabase](https://www.supabase.com) - Fully managed Postgres with read replicas, point-in-time-recovery, support packages, browser based GUI, and a generous free tier.
* [Neon](https://neon.tech) - Fully managed serverless PostgreSQL. Neon separates storage and compute to offer modern developer features such as serverless, branching, bottomless storage, and more.
* [Nile](https://www.thenile.dev/) - Fully managed PostgreSQL . Nile decouples storage from compute and virtualizes tenants to ship multi-tenant AI applications fast, safe, and with limitless scale. Free tier provides unlimited databases.
* [Vela](https://vela.run) - Postgres-based backend-as-a-service built for modern AI apps. Offers instant database branches and clones, production-like test environments, and serverless scaling.
* [Thalassa Cloud DBaaS](https://thalassa.cloud/products/databases/postgresql/) - Fully managed PostgreSQL database, multi-AZ, automated backups, hosted in the Netherlands.

### Docker images

* [citusdata/citus](https://hub.docker.com/r/citusdata/citus/) - Citus official images with citus extensions. Based on the official Postgres container.
* [mdillon/postgis](https://hub.docker.com/r/mdillon/postgis/) - PostGIS 2.3 on Postgres 9. Based on the official Postgres container.
* [paradedb/paradedb](https://hub.docker.com/r/paradedb/paradedb/) - ParadeDB is Postgres for Search and Analytics. Based on the official Postgres container with pg\_search extension.
* [postgres](https://hub.docker.com/_/postgres/) -  Official postgres container (from Docker)

### Kubernetes

* [CloudNativePG operator](https://github.com/cloudnative-pg/cloudnative-pg) ⭐ 8,024 | 🐛 310 | 🌐 Go | 📅 2026-02-16 - A comprehensive platform designed to seamlessly manage PostgreSQL databases within Kubernetes environments.
* [Zalando Operator](https://github.com/zalando/postgres-operator) ⭐ 5,084 | 🐛 554 | 🌐 Go | 📅 2026-02-13 - Creates and manages PostgreSQL clusters running in Kubernetes.
* [Crunchy Operator](https://github.com/CrunchyData/postgres-operator) ⭐ 4,367 | 🐛 145 | 🌐 Go | 📅 2026-02-13 - Production PostgreSQL for Kubernetes, from high availability Postgres clusters to full-scale database-as-a-service.
* [StackGres Operator](https://github.com/ongres/stackgres/) ⭐ 1,362 | 🐛 1 | 🌐 Java | 📅 2026-02-15 -  Full Stack PostgreSQL on Kubernetes.
* [Kubegres Operator](https://github.com/reactive-tech/kubegres) ⭐ 1,353 | 🐛 79 | 🌐 Go | 📅 2025-01-04 - Kubegres is a Kubernetes operator allowing to deploy one or many clusters of PostgreSql instances and manage databases replication, failover and backup.
* [Percona PostgreSQL Operator](https://github.com/percona/percona-postgresql-operator) ⭐ 355 | 🐛 31 | 🌐 Go | 📅 2026-02-15 - Percona Operator for PostgreSQL based on Crunchy Data operator.
* [Percona Everest Operator](https://github.com/percona/everest-operator) ⭐ 38 | 🐛 19 | 🌐 Go | 📅 2026-02-10 - Everest Operator is a Kubernetes Operator responsible for managing the lifecycle of MySQL, MongoDB, and PostgreSQL databases. It leverages Percona's Kubernetes Operators for MySQL, MongoDB, and PostgreSQL under the hood but provides a unified API and a single pane of glass for managing all three database types.
* [Fujitsu Enterprise Postgres for Kubernetes](https://www.postgresql.fastware.com/) - Enterprise-grade PostgreSQL on OpenShift Container Platform (Commercial Software).
* [KubeDB operator](https://kubedb.com/) - Run Production-Grade Databases on Kubernetes (Commercial Software).

## Resources

### Tutorials

* [pg-utils](https://github.com/dataegret/pg-utils) ⭐ 1,186 | 🐛 6 | 🌐 Shell | 📅 2025-12-05 - Useful DBA tools by Data Egret
* [postgresDBSamples](https://github.com/morenoh149/postgresDBSamples) ⭐ 544 | 🐛 1 | 🌐 PLpgSQL | 📅 2023-09-20 - A collection of sample postgres schemas
* [pagila](https://github.com/xzilla/pagila) ⭐ 70 | 🐛 1 | 🌐 PLpgSQL | 📅 2025-06-05 - Pagila, Postgres Sample Database
* [Backup and recover a PostgreSQL DB using wal-e](https://coderwall.com/p/cwe2_a/backup-and-recover-a-postgres-db-using-wal-e) - Tutorial about setting up continuous archiving in PostgreSQL using wal-e.
* [Operations cheat sheet](https://wiki.postgresql.org/wiki/Operations_cheat_sheet) - Operations cheat sheet from PostgreSQL Wiki.
* [PG Casts](https://www.pgcasts.com) - Free weekly PostgreSQL screencasts by Hashrocket.
* [Postgres Guide](http://postgresguide.com/) - Guide designed as an aid for beginners and experienced users to find specific tips and explore tools available within PostgreSQL.
* [PostgreSQL Exercises](https://pgexercises.com/) - Site  to make it easy to learn PostgreSQL by doing exercises.
* [tutorialspoint PostgreSQL tutorial](http://www.tutorialspoint.com/postgresql/) - Very extensive collection of tutorials on PostgreSQL
* [PostgreSQL Primer for Busy People](https://zaiste.net/posts/postgresql-primer-for-busy-people/) - A collection of the most common commands used in PostgreSQL

### Blogs

* [Planet PostgreSQL](https://planet.postgresql.org/) - Blog aggregation service for PostgreSQL.
* [Andrew Dunstan's PostgreSQL and Technical blog](http://adpgtech.blogspot.com/search/label/PostgreSQL/)
* [Bruce Momjian's PostgreSQL blog](https://momjian.us/main/blogs/pgblog.html)
* [Craig Kerstiens PostgreSQL posts](http://www.craigkerstiens.com/categories/postgres/) - Set of posts on PostgreSQL cool features, tips and tricks.
* [Database Soup](http://www.databasesoup.com/search/label/postgresql/) - Josh Berkus' blog.
* [Michael Paquier's blog](https://paquier.xyz/)
* [Percona's PostgreSQL blog posts](https://www.percona.com/blog/category/postgresql/)
* [Robert Haas' blog](http://rhaas.blogspot.com/search/label/postgresql/)
* [select \* from depesz;](https://www.depesz.com/tag/postgresql/) - Hubert Lubaczewski's blog.
* [Metis Blog](https://www.metisdata.io/blog) - Set of posts on PostgreSQL, SQL databases, performance, and tuning.
* [Digoal's PostgreSQL and Technical blog(Chinese Language)](https://github.com/digoal/blog/blob/master/README.md) ⭐ 8,427 | 🐛 66 | 🌐 PLpgSQL | 📅 2026-02-13
* [Pigsty blog / PostgreSQL](https://pigsty.io/blog/pg/) - Blog by the author of PIGSTY with insightful articles on PostgreSQL (as well as databases and cloud infrastructure).

### Books

* [PostgreSQL Mistakes and How to Avoid Them](https://www.manning.com/books/postgresql-mistakes-and-how-to-avoid-them)
* [The Internals of PostgreSQL](https://www.interdb.jp/pg/index.html) - A free e-book by Hironobu Suzuki
* [PostgreSQL 14 Internals](https://postgrespro.com/community/books/internals) - A free e-book by Egor Rogov

### Documentation

* [Wiki](https://wiki.postgresql.org/wiki/Main_Page) - user documentation, how-tos, and tips 'n' tricks
* [pgPedia](https://pgpedia.info/) - An encyclopedia of things related to postgreSQL.
* [create\_pg\_super\_document](https://ryogrid.github.io/create_pg_super_document/index.html) - A project that aim to generate documentation for all symbols in the PostgreSQL codebase using AI agents

### Newsletters

* [Postgres Weekly](https://postgresweekly.com/) - Weekly newsletter that contains articles, news, and repos relevant to PostgreSQL.
* [pgMustard newsletter](https://www.pgmustard.com/newsletter) - Monthly newsletter that contains Postgres performance articles and videos.

### Podcasts

* [PostgresFM](https://postgres.fm/) - Weekly discussions about Postgres topics.
* [Scaling Postgres](https://www.scalingpostgres.com/) - Weekly roundups of PostgreSQL related content.
* [Path to Citus Con](https://www.citusdata.com/podcast/path-to-citus-con/) - Monthly interviews with people in the Postgres world.

### Videos

* [Citus Data Youtube channel](https://www.youtube.com/channel/UC8jpoK1BqQhDh6HDGFnM_DA/videos) - Citus related videos
* [EnterpriseDB Youtube channel](https://www.youtube.com/channel/UCkIPoYyNr1OHgTo0KwE9HJw) -  EnterpriseDB related videos
* [Postgres Conference Youtube channel](https://www.youtube.com/channel/UCsJkVvxwoM7R9oRbzvUhbPQ/videos) - Conference videos
* [Scaling Postgres](https://www.scalingpostgres.com/) - Postgres video blog series by Creston Jamison
* [PostgresTV Youtube channel](https://www.youtube.com/@PostgresTV) - Postgres talks, hacking sessions, interviews, and podcast episodes

### Community

* [Mailing lists](https://www.postgresql.org/list/) - Official mailing lists for Postgres for support, outreach, and more. One of the primary channels of communication in the Postgres community.
* [Reddit](https://www.reddit.com/r/PostgreSQL/) - A reddit community for PostgreSQL users with over 12000 users
* [Slack](https://pgtreats.info/slack-invite) - Slack workspace for Postgres with over 20k members
* Telegram - Several groups for PostgreSQL in different languages: [Russian](https://t.me/pgsql) >4200 people, [Brazilian Portuguese](https://t.me/postgresqlbr) >2300 people, [Indonesian](https://t.me/postgresql_id) \~1000 people, [English](https://t.me/postgreschat) >750 people
* [#postgresql on Freenode](https://webchat.freenode.net/#postgresql) - The most popular IRC channel about Postgres on Freenode with over 1000 users
* [Discord](https://discord.gg/bW2hsax8We) - A Discord server for Postgres with over 6k members

### Roadmaps

* [PostgreSQL Roadmap](https://roadmap.sh/postgresql-dba) - A roadmap providing step wise guide to PostgreSQL.

### External lists

* [Wikipedia admin tools list](https://en.wikipedia.org/wiki/Comparison_of_database_tools) - Comparison of database administration tools on Wikipedia
* [PostgreSQL Wiki GUI tools list](https://wiki.postgresql.org/wiki/Community_Guide_to_PostgreSQL_GUI_Tools) - Community Guide to PostgreSQL GUI Tools
* [PostgreSQL Wiki Foreign Data Wrappers list](https://wiki.postgresql.org/wiki/Foreign_data_wrappers) - Foreign data wrappers
