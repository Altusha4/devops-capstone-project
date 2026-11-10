# Submission status — 2026-11-10

- Customer Accounts REST API implements create, read, update, delete and list.
- Local PostgreSQL test run passed with 95% coverage. Red-phase test output is retained locally.
- GitHub CI passed: https://github.com/Altusha4/devops-capstone-project/actions/runs/42820718905
- Security headers and restricted CORS are covered by tests.
- Docker image runs as a non-root user.
- Actual local Kubernetes deployment is in the isolated `devops-capstone` namespace of Minikube, backed by PostgreSQL.
- Tekton PipelineRun `accounts-cd-9hwqj` succeeded: clone, lint/test, Kaniko build/push and deployment rollout. Pipeline tests use SQLite; local and GitHub CI tests use PostgreSQL.
- `tekton/local-pipeline.yaml` is the executable local pipeline. `deploy/registry.yaml` supplies an isolated laboratory registry. HTTP and disabled HTTPS redirects are for this local lab only, not a production configuration.
- Evidence files are local and excluded from Git. No credentials are committed.
- Story points are displayed as `[SP: n]` in issue titles and described in issue bodies.
- Planning screenshots show the exercise board; the labels/backlog arrangement was recaptured for documentation after implementation. Milestone dates are planning exercise dates, not elapsed work durations.
- Final assessment is prepared as a draft for learner review; no score or certificate is claimed.
