# Technical Debt

Repository-wide technical debt cannot be rated solely from file counts. Candidate review areas are large inheritance surfaces, optional integration configuration, route authorization consistency, generated/runtime schema drift, migration completeness, test isolation, and deployment-specific observability. Findings should be validated with linting, tests, profiling, dependency scanning, and a selected production-like module/database configuration.
