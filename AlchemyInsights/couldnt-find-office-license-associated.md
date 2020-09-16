---
title: A Microsoft 365-alkalmazások kijavítása nem talált Office-licenceket a kapcsolódó üzenetekhez
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747697"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>A Microsoft 365-alkalmazások rögzítése "nem található az Office-licencek társított" üzenet

Ha ez az üzenet jelenik meg, próbálkozzon az alábbiakkal:

1. Ellenőrizze a tűzfal, a víruskereső szoftverek és a proxybeállítások között, és győződjön meg arról, hogy a Microsoft 365-alkalmazásokban nem akadályozza meg az internet elérését. Lásd: [Microsoft 365 URL-EK és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Az érintett felhasználó [Office-licencének](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) eltávolítása és hozzárendelése. 
3. Nyisson meg egy Office-alkalmazást, és [kijelentkezhet](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) a meglévő felhasználói fiókokból.
4. Válassza a Windows-beállítások > **fiókok**  >  **e-mail-&-fiókjai**lehetőséget, és távolítsa el az összes munkafiókot, kivéve az érintett fiókot.
5. Nyissa meg a Windows beállításai > **fiókokhoz**  >  **való hozzáférést (munkahelyi vagy iskolai**), és válassza le az összes munkafiókját, kivéve az érintett fiókot.
6. Állítsa vissza az Office aktiválási állapotát. [További információ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Bejelentkezés](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.

További hibaelhárítási megoldásokat a nem [licencelt termék-és aktiválási hibák az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)című témakörben találhat.