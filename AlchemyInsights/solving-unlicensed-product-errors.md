---
title: "\"Nem licencelt termék\" hibaüzenetek megoldása"
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786851"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Javaslatok a "Nem licencelt termék" hibaüzenetek megoldásához

A "Nem licencelt termék" hibaüzenetek megoldásához próbálkozzon az alábbiakkal:

- Ellenőrizze, hogy lejárt-e az előfizetés állapota.
- Győződjön meg arról, hogy olyan előfizetése van, amely lehetővé teszi az ügyféllicenceket, például a Microsoft 365 Vállalati verziós appokat vagy a Vállalati prémium verzió használatát, és győződjön meg arról, hogy a felhasználóhoz licenc van [rendelve.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Győződjön meg arról, hogy a felhasználó ugyanazokkal a fiókkal jelentkezik be az Office-be, mint amelyhez a licenc van hozzárendelve.
- Ellenőrizze a [Szolgáltatás állapota lapon,](https://docs.microsoft.com/office365/enterprise/view-service-health) hogy nincs-e bármilyen ismert probléma a szolgáltatással kapcsolatban.
- Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem gátolja meg a Microsoft 365-alkalmazások internetelérését. Lásd: [URL-ek és IP-címtartományok.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

A következő hibaelhárítási műveletekkel is próbálkozhat: 

- Nyisson meg egy Office-appot, [és jelentkezzen](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ki a meglévő felhasználói fiókokból. [Távolítsa](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [el, majd rendelje](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) hozzá újra az Office-licencet, majd jelentkezzen be az [Office-be](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.
- Futtassa az [Aktiválási hibaelhárítót.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Végezze el az Office online javítását.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

További hibaelhárítási megoldásért lásd: 

- [„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)