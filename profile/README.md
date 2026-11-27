# Finance Lab

Finance Lab is a personal finance app for planning a month in rubles and reviewing how it went. The Russian-language interface works on desktop and phone. Enter income, category spending and investment contributions, then compare the saved months in a yearly report.

[Try the local demo](https://github.com/finance-lab-project/finance-lab#run-the-local-fixture) · [Latest release](https://github.com/finance-lab-project/finance-lab/releases/latest) · [Owner sign-in](https://finance-lab-project.com/)

The hosted instance serves one configured owner. The local demo uses disposable accounts and a sample budget.

## Application and architecture

The [application repository](https://github.com/finance-lab-project/finance-lab) contains the Java and Spring Boot application, Thymeleaf screens and SQLite storage. The [implementation decision](https://github.com/finance-lab-project/finance-lab/blob/main/docs/implementation-approach.md) explains why this design fits the monthly budgeting workflow. The [release notes](https://github.com/finance-lab-project/finance-lab/releases) record the features available in each published version.

## How changes reach production

The maintainer authorizes sprint work through GitHub issues. For work handled by the sprint worker, Codex implements a change and a separate review session checks the pull request. GitHub requires passing CI and approval before merge. Deployment takes place during a separate maintenance window with backup and verification checks.

[Sprint board](https://github.com/orgs/finance-lab-project/projects/11/views/1) · [Sprint worker](https://github.com/finance-lab-project/finance-lab/blob/main/ops/agents/README.md) · [Release process](https://github.com/finance-lab-project/finance-lab#releases)

## Project history

The earlier Java/Vaadin and PostgreSQL implementation is archived in the [application](https://github.com/finance-lab-project/app), [Budget module](https://github.com/finance-lab-project/budget) and [custom ORM](https://github.com/finance-lab-project/orm) repositories. The archived [Portfolio](https://github.com/finance-lab-project/portfolio) and [FIRE](https://github.com/finance-lab-project/fire) repositories preserve module plans from that iteration.
