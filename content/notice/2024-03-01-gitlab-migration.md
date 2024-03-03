---
title: "2024-03-01 Gitlab Migration"
date: 2024-01-31T15:57:13+09:00
draft: false
---

As of the end of February, SiliconForest GitLab will migrate from GitLab to Forgejo and be renamed SiliconForest Atelier.

The primary reasons for migration are:

* Forgejo supports a free search feature, while GitLab does not.
* Forgejo will get the most decent federation feature
* Forgejo is written in Go, which will be much lighter compared to RoR-based GitLab

Breaking changes will be:

* SiliconForest Atelier will no longer maintain an authentication database and will solely rely on SSO to authenticate a user
* SiliconForest Atelier will not provide GitLab CI but will integrate Woodpecker CI.
* SiliconForest Atelier will be viewable by the public.

The migration plan is as follows:

* ~~On **2024-03-01**, SiliconForest GitLab will moved to `git-old.silicon.moe`, and a new Forgejo instance will launched at `git.silicon.moe`~~ **2024-03-03**, SiliconForest GitLab moved to **git-old.silicon.moe** and Forgejo is online at **git.silicon.moe**
* **`git-old.silicon.moe` will be offline after three months (2024-06-01)**. You are responsible for migrating the repository or taking the backup in time.
* SiliconForest will accept SiliconForest ID requests for current GitLab users without SiliconForest ID during those **three months** but will **no longer accepted after that**.

If you have any questions about the migration, please get in touch with the admin via [Fediverse account](https://social.silicon.moe/@perillamint) or `@perillamint:silicon.moe` Matrix account.
