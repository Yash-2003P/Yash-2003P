## Yash

RHCSA & RHCE certified. Linux and DevOps engineer working across RHEL/Ubuntu, Ansible and Bash,
and contributing to [Kestra](https://github.com/kestra-io/kestra) — the declarative orchestration
engine for data workflows.

### Open Source Contributions

[![Contributor](https://img.shields.io/badge/2%20PRs%20MERGED-KESTRA-1F232C?style=for-the-badge&logo=github&logoColor=200062&labelColor=CDC5FF)](https://github.com/search?q=org:kestra-io+author:Yash-2003P+is:pr+is:merged&type=pullrequests)

### Merged pull requests to Kestra

- **refactor(executions): replace explicit any in ExecutionRoot.vue and useExecutionRoot.ts**
  ([#20417](https://github.com/kestra-io/kestra/pull/20417)) — removed the two explicit `any` on
  the execution root page, finishing [#20332](https://github.com/kestra-io/kestra/issues/20332).
  `useExecutionRoot.follow()` was passing the whole `route.params` object into
  `followExecution({id})`, so the extra `namespace`/`flowId` keys were dead weight and the cast
  was hiding the excess-property error that would have flagged it; it now passes the execution id
  alone. `ExecutionRoot.vue` no longer casts `routeInfo` before `useRouteContext`, because both
  branches of that computed already produce a string title. Both files drop out of the
  `explicit-any` baseline the project keeps under `ui/scripts/explicit-any/`.
- **refactor(ui): replace the text-success Bootstrap utility in AddTriggerModal.vue**
  ([#21145](https://github.com/kestra-io/kestra/pull/21145)) — swapped a Bootstrap utility class
  for the design system's own token.

### Stack

**Kestra** — Java 25, Micronaut, jOOQ, Gradle, JUnit 5, AssertJ on the backend; Vue 3,
TypeScript, Vite, Pinia, Vitest and Playwright on the frontend; H2, PostgreSQL and MySQL for
persistence.

**Linux & DevOps** — RHEL and Ubuntu, Ansible, Bash, systemd, Nginx, Docker and cloud
infrastructure.

**Also** — Python, Node.js/Express, Go and Rust.

### Pinned work

- [linux-infra-intern-lab](https://github.com/Yash-2003P/linux-infra-intern-lab) — Ubuntu Server
  baseline lab with Bash automation, Nginx, systemd, UFW, validation scripts and hardening notes.
- [LeapAI-Assist](https://github.com/Yash-2003P/LeapAI-Assist) — AI-native onboarding assistant for
  openSUSE Leap.
- [College-Appointment-System](https://github.com/Yash-2003P/College-Appointment-System) —
  Node.js/Express appointment API with JWT roles and MongoDB, deployed on EC2 + DocumentDB.
