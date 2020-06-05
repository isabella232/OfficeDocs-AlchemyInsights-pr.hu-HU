---
title: Nem licencelt termékhibák megoldása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 89d0e589329d40f17c36baa54868154be0f5b887
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582741"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Javaslatok a "Nem licencelt termék" hibák megoldására

A "Nem licencelt termékkel" kapcsolatos hibák megoldásához próbálkozzon az alábbiakkal:

- Ellenőrizze, hogy lejárt-e az előfizetésállapota.
- Győződjön meg arról, hogy rendelkezik olyan előfizetéssel, amely lehetővé teszi az ügyféllicencek használatát, például a Microsoft 365 Vállalati verziók vagy a Business Premium alkalmazást, és [győződjön meg arról, hogy a felhasználó rendelkezik-e licenccel.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Győződjön meg arról, hogy a felhasználó ugyanazzal a fiókkal jelentkezik be az Office-ba, amelyhez a licenc hozzá van rendelve.
- Ellenőrizze a [Szolgáltatás állapotlapján,](https://docs.microsoft.com/office365/enterprise/view-service-health) hogy vannak-e ismert problémák a szolgáltatással.
- Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és ellenőrizze, hogy azok nem akadályozzák-e a Microsoft 365 alkalmazások internet-hozzáférését. Lásd [URL-címek és IP-címtartományok](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Próbálkozzon a következő hibaelhárítási műveletekkel is: 

- Nyisson meg egy Office-alkalmazást, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) a meglévő felhasználói fiókokból. [Távolítsa el](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) és rendelje hozzá újra az Office-licencet, majd jelentkezzen be az [Office-ba](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) az érintett felhasználói fiókkal. [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)
- Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Az Office online javításának végrehajtása.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

További hibaelhárítási megoldásért lásd: 

- [„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)