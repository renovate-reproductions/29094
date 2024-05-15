# Renovate minimal repoduction
Temporary repo to troubleshoot Renovate


## Current behaviour

Renovate only update semiversion create PRs for updates to newer revisions within the same Debian release, such as:

```
-FROM docker.io/bitnami/redis:7.2.3-debian-11-r0
+FROM docker.io/bitnami/redis:7.2.4-debian-11-r0
```

New update to revisions are ignored

## Expected behaviour

```
-FROM docker.io/bitnami/redis:7.2.4-debian-11-r12
+FROM docker.io/bitnami/redis:7.2.4-debian-11-r15
```