---
title: A Microsoft 365-appok nem található az Office-licencekkel társított üzenet kijavítva
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816490"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>A "Nem található a kapcsolódó Office-licencek" üzenet kijavítja a Microsoft 365-appokat.

Ha megjelenik ez az üzenet, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem gátolja meg a Microsoft 365-alkalmazásokhoz való internet-hozzáférést. Lásd: [A Microsoft 365 URL-címei és IP-címtartományai.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Távolítsa [el,](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) majd vegye ki újra az érintett felhasználó Office-licencét. 
3. Nyisson meg egy Office-appot, [és jelentkezzen](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ki a meglévő felhasználói fiókokból.
4. A Windows beállításai lapon > **fiókok**  >  **e-mail & fiókokat,** és távolítsa el az összes munkahelyi fiókot, kivéve az érintett fiókot.
5. Válassza a Windows Beállításai > **Fiókok Hozzáférés** munkahelyi vagy iskolai fiókjához lehetőséget, és válassza le az érintett fiókon kívül az összes munkahelyi  >  fiókot.
6. Állítsa vissza az Office aktiválási állapotát. [További információ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Jelentkezzen be](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.

További hibaelhárítási megoldásokat a "Nem licencelt termék" aktiválási hibaüzenetek [az Office-ban témakörben talál.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)