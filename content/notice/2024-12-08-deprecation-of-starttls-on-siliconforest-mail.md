---
title: "2024-12-08 Deprecation of STARTTLS on SiliconForest Mail"
date: 2024-09-08T14:37:00+09:00
draft: false
---

Due to [security concerns on STARTTLS](https://nostarttls.secvuln.info/), [Mailu disabled STARTTLS ports by default](https://mailu.io/master/releases.html#mailu-2024-06-2024-06).
This change affects SiliconForest mail, which uses Mailu to provide service.

To reduce the impact of this change, SiliconForest Mail chose to force-enable the STARTTLS port for three months.

All users who rely on STARTTLS port (TCP 587 SMTP, TCP 143 IMAP) MUST change their configuration to use SMTPS (TCP 465) and IMAPS (TCP 993) before 2024-12-08.

If you have any questions about the change, please contact the admin via [Fediverse account](https://social.silicon.moe/@perillamint) or `@perillamint:silicon.moe` Matrix account.
