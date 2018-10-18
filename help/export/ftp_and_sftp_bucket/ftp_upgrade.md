---
description: Upgrades to Adobe FTP servers can introduce new configurations that affect automation scripts (often used to download or upload data regularly), which are often built to rely on certain server settings.
keywords: ftp;sftp
seo-description: Upgrades to Adobe FTP servers can introduce new configurations that affect automation scripts (often used to download or upload data regularly), which are often built to rely on certain server settings.
seo-title: Upgrade Adobe FTP servers
solution: Analytics
title: Upgrade Adobe FTP servers
uuid: 3572c65c-a6e2-4120-b89a-7f43428144ed
index: y
internal: n
snippet: y
---

# Upgrade Adobe FTP servers

Upgrades to Adobe FTP servers can introduce new configurations that affect automation scripts (often used to download or upload data regularly), which are often built to rely on certain server settings.

For example, a new success status is introduced, affecting a script that uses the success status to trigger a certain action. Adobe pro-actively notifies users of such configuration changes. If Adobe notifies you that an FTP server upgrade is imminent, check your automation scripts to make sure they are still working correctly. 