# SQLBenchmark

Evaluating Microsoft SQL Server performance using TPC-DS (Decision Support) and TPC-DI (Data Integration) benchmarks.

## The Problem

- Selecting a database platform for analytical workloads requires objective performance evidence, not vendor claims.
- TPC benchmarks provide a standardised, reproducible methodology for comparing query throughput and data loading performance.
- Establishing a performance baseline for MS SQL Server informs architecture decisions for data warehouse projects.

## The Approach

**Inputs:** TPC-DS and TPC-DI benchmark datasets and query sets, stored in `data/`. Reference materials are in `references/`.

**Processing:** SQL scripts in `src/` execute benchmark workloads against a local MS SQL Server instance. Results are recorded and compared against expected TPC metrics.

**Outputs:** Performance measurements for MS SQL Server under decision-support and data-integration workloads.

## Value Delivered

- Provides reproducible benchmark results for MS SQL Server on the TPC-DS and TPC-DI suites.
- Supports data platform selection decisions with empirical performance data.

## Scope & Status

- **Project type:** Research / academic benchmarking
- **Current state:** Archived
- **Known limitations:**
  - Results are environment-specific; hardware and configuration will affect outcomes.
  - No automated test runner; steps must be executed manually.

## Tech Stack

- **Database:** Microsoft SQL Server
- **Language:** T-SQL
- **Benchmark suites:** TPC-DS, TPC-DI

## Who This Is For

Data engineers and architects evaluating MS SQL Server for analytical workloads. Reviewers assessing the author's database benchmarking experience.

## Related Work

- [TPC-DI-MS-SQL-Benchmark](https://github.com/abroniewski/TPC-DI-MS-SQL-Benchmark) — a more detailed project focused specifically on the TPC-DI benchmark with ETL scripts.

## License

Not specified.
