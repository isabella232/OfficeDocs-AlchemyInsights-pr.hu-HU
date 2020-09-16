---
title: Nem licencelt termékkel kapcsolatos hibák megoldása
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737955"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Javaslatok a "nem licencelt termék" hibák megoldására

A "nem licencelt termék" hibáinak elhárításához próbálkozzon az alábbiakkal:

- Ellenőrizze, hogy az előfizetés állapota lejárt-e.
- Ellenőrizze, hogy rendelkezik-e olyan előfizetéssel, amely lehetővé teszi az ügyfélalkalmazások (például a Microsoft 365-alkalmazások vállalati verziós vagy vállalati prémium verzió) használatát, és győződjön meg arról, [hogy a felhasználó rendelkezik licenccel](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Ügyeljen arra, hogy a felhasználó ugyanazzal a fiókkal jelentkezzen be az Office-ba, amelyhez licenc van rendelve.
- A [szolgáltatás állapota lapon](https://docs.microsoft.com/office365/enterprise/view-service-health) ellenőrizheti, hogy vannak-e ismert problémák a szolgáltatással kapcsolatban.
- Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat annak megerősítéséhez, hogy ne blokkolja a Microsoft 365-alkalmazásokat az internethez. Lásd: [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Az alábbi hibaelhárítási műveleteket is elvégezheti: 

- Nyisson meg egy Office-alkalmazást, és [kijelentkezhet](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) a meglévő felhasználói fiókokból. [Távolítsa el](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) , majd [rendelje újra](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) az Office-licencet, majd az érintett felhasználói fiókkal [bejelentkezhet az Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) -ba.
- Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Végezze el az Office Online javítását](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

További hibaelhárítási megoldásért lásd: 

- [„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)