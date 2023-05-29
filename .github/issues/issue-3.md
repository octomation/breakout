---
code: null
id: I_kwDOFMiCZ87wrJGA
databaseId: 4037841280
number: 3
url: https://github.com/octomation/breakout/issues/3
title: "deps: ansible warnings"
issueType: Bug
labels:
  - "difficulty: easy"
  - "kind: bug"
  - "kind: improvement"
  - "level: low"
  - "scope: code"
assignees:
  - kamilsk
milestone: null
parent: null
issueFields: {}
state: CLOSED
stateReason: COMPLETED
duplicateOf: null
createdAt: 2026-03-07T08:14:23Z
updatedAt: 2026-04-17T18:01:53Z
lastEditedAt: null
closedAt: 2026-04-17T18:01:53Z
---

# deps: ansible warnings

**Details**

```
[WARNING]: Deprecation warnings can be disabled by setting `deprecation_warnings=False` in ansible.cfg.
[DEPRECATION WARNING]: INJECT_FACTS_AS_VARS default to `True` is deprecated, top-level facts will not be auto injected after the change. This feature will be removed from ansible-core version 2.24.
Origin: /.../octomation/vpn/ansible/roles/docker/tasks/engine.yml:10:21

 8 - name: Set up the stable repository
 9   apt_repository:
10     repo:           deb [arch=amd64] https://download.docker.com/linux/ubuntu {{ ansible_lsb.codename }} stable
                       ^ column 21

Use `ansible_facts["fact_name"]` (no `ansible_` prefix) instead.
```

```
[DEPRECATION WARNING]: INJECT_FACTS_AS_VARS default to `True` is deprecated, top-level facts will not be auto injected after the change. This feature will be removed from ansible-core version 2.24.
Origin: /.../octomation/vpn/ansible/roles/docker/tasks/compose.yml:14:11

12 - name: Install docker-compose
13   get_url:
14     url:  https://github.com/docker/compose/releases/download/{{ docker_compose_version }}/docker-compose-{{ ansib...
             ^ column 11

Use `ansible_facts["fact_name"]` (no `ansible_` prefix) instead.
```

<!-- 2026-04-17T18:01Z https://github.com/octomation/breakout/issues/3#issuecomment-4270200172
fixed
-->
