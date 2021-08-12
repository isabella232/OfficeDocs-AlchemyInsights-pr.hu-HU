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
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957102"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Javaslatok a "Nem licencelt termék" hibaüzenetek megoldásához

A "Nem licencelt termék" hibaüzenetek megoldásához próbálkozzon az alábbiakkal:

- Ellenőrizze, hogy lejárt-e az előfizetés állapota.
- Győződjön meg arról, hogy olyan előfizetése van, amely lehetővé teszi az ügyféllicencek Üzleti Microsoft 365-alkalmazások a Prémium vállalati verzió, és hogy a felhasználóhoz licenc van [rendelve.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Győződjön meg arról, hogy a felhasználó a Office társított fiókkal jelentkezik be az alkalmazásba.
- Ellenőrizze a [Szolgáltatás állapota lapon,](https://docs.microsoft.com/office365/enterprise/view-service-health) hogy nincs-e bármilyen ismert probléma a szolgáltatással kapcsolatban.
- Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy azok nem Microsoft 365 az appok internet-hozzáférését. Lásd: [URL-ek és IP-címtartományok.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

A következő hibaelhárítási műveletekkel is próbálkozhat: 

- Nyisson [Office-app, és jelentkezzen](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ki a meglévő felhasználói fiókokból. [Távolítsa](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [el,](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) majd rendelje hozzá újra a Office, majd jelentkezzen be Office [az](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) érintett felhasználói fiókkal.
- Futtassa az [Aktiválási hibaelhárítót.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Végezze el a Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)online javítását.

További hibaelhárítási megoldásért lásd: 

- [„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)