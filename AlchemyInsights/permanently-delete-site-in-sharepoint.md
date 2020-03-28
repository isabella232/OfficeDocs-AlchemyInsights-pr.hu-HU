---
title: Webhely végleges törlése a SharePointban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955168"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Webhely végleges törlése a SharePointban

Ha újra fel szeretne használni egy URL-t egy törölt webhelyről (a webhely újbóli létrehozásához), vagy véglegesen törölni szeretné a webhelyet, mert az már nincs használatban, akkor használja az új SharePoint felügyeleti központból a **Végleges törlés** opciót. 

1. Nyissa meg az [Új SharePoint felügyeleti központ törölt helyek lapját](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) és jelentkezzen be egy olyan fiókkal, amely rendszergazdai engedélyekkel rendelkezik a szervezetéhez. 

2. A bal oldali oszlopban válasszon ki egy webhelyet. 

3. Kattintson a **Végleges törlés**elemre. 

**Megjegyzés**: a csoportosított webhely nem törölhető véglegesen az új SharePoint felügyeleti központból. Ehelyett a [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) használata szükséges.  

További információt a [Webhely végleges törlése](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) témakörben talál. 
