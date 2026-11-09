# Finance Lab

Personal finance software, starting with monthly budgeting.

Finance Lab is a personal product and engineering project. Budget is the first business module; investment portfolio analysis and financial-independence planning (FIRE) are planned for later.

**Start with [app](https://github.com/finance-lab-project/app)** for the application, setup instructions and project documentation.

## Current focus

The Budget implementation covers monthly RUB planning, configurable spending categories, explicit saves and read-only recorded history, with a Russian-language interface. The application assembly includes a browser-local guest planner and an authenticated PostgreSQL Budget workspace.

The current architecture is a Java/Vaadin modular monolith without Spring, backed by PostgreSQL Anchor Modeling and a custom ORM. The first release targets one configured account with no public registration. Public source repositories do not imply public access to account data.

The MVP is undergoing [technical review](https://github.com/finance-lab-project/app/blob/main/docs/review/README.md). That review records implementation evidence, known findings and remaining deployment and operational acceptance gaps.

## Repositories

| Repository | Purpose | Status |
| --- | --- | --- |
| [app](https://github.com/finance-lab-project/app) | Application assembly, authentication, configuration and shared documentation | Current application |
| [budget](https://github.com/finance-lab-project/budget) | Monthly planning, categories, Vaadin UI, persistence and recorded history | First business module |
| [orm](https://github.com/finance-lab-project/orm) | Custom Anchor mapper, JDBC transactions, SQL generation and history projections | Supporting library |
| [portfolio](https://github.com/finance-lab-project/portfolio) | Planned holdings, investment transactions and portfolio calculations | Planning only; deferred beyond Budget R1 |
| [fire](https://github.com/finance-lab-project/fire) | Planned financial-independence goals, assumptions and projections | Planning only; deferred beyond Budget R1 |

## Documentation and progress

- [Technical review and evidence](https://github.com/finance-lab-project/app/blob/main/docs/review/README.md)
- [Architecture and agreed contracts](https://github.com/finance-lab-project/app/blob/main/docs/architecture.md)
- [Release plan](https://github.com/finance-lab-project/app/blob/main/docs/roadmap.md)
- [Budget R1 release tracker](https://github.com/finance-lab-project/app/issues/1)

For development, begin with the relevant repository's README and `AGENTS.md`. Use synthetic financial data in examples, tests, issues and pull requests. Human review and approval are required before merge, release or deployment.

## Project history

The archived [frontend](https://github.com/finance-lab-project/frontend), [budget-service](https://github.com/finance-lab-project/budget-service), [platform](https://github.com/finance-lab-project/platform) and [web-bff](https://github.com/finance-lab-project/web-bff) repositories preserve earlier work. Their React, Go/BFF and infrastructure directions are historical.
