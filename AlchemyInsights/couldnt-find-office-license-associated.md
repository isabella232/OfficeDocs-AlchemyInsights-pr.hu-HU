---
title: A Microsoft 365-alkalmazások javítása Nem található az irodai licencekkel társított üzenet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580443"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>A Microsoft 365 alkalmazás "Nem található irodai licencek nem találhatók" üzenetének javítása

Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e a Microsoft 365-alkalmazások internet-hozzáférését. Lásd: [Microsoft 365 URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Távolítsa el és [rendelje hozzá újra az Office-licencet](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) az érintett felhasználószámára. 
3. Nyisson meg egy Office-alkalmazást, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) a meglévő felhasználói fiókokból.
4. Nyissa meg a Windows > **Fiókok**  >  **e-mail fiókok & a fiókokat,** és távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot.
5. Nyissa meg a **Accounts**Windows-beállítások >  >  **Fiókok: Munkahelyi vagy iskolai hozzáférés,** és az érintett fiók kivételével az összes munkahelyi fiók leválasztása.
6. Állítsa vissza az Office aktiválási állapotát. [További információ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Jelentkezzen be](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.

További hibaelhárítási megoldásokat az [Office Nem licencelt termék- és aktiválási hibái című témakörben talál.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)