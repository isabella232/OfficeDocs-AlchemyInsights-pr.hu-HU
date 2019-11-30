---
title: Nem licencelt Termékhibák megoldása
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
ms.openlocfilehash: 178811c81775b22676a0106283be4e516d40a95b
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628028"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Javaslatok a "nem licencelt termék" hibáinak megoldására

Egy "nem licencelt termék" hibáinak elhárításához próbálkozzon a következőkkel:

- Ellenőrizze, hogy lejárt-e az előfizetési állapot.
- Győződjön meg arról, hogy rendelkezik olyan előfizetéssel, amely lehetővé teszi az ügyféllicencek (például az Office 365 Business vagy Business Premium) számára, és [biztosítja, hogy a felhasználónak van hozzárendelve licence](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users). 
- Győződjön meg arról, hogy a felhasználó bejelentkezik az Office-ba ugyanazzal a fiókkal, amely a licencet kiosztta.
- Ellenőrizze az [Office 365 szolgáltatás-egészségügyi lapon](https://docs.microsoft.com/office365/enterprise/view-service-health) , hogy vannak-e a szolgáltatással kapcsolatos ismert problémák.
- Ellenőrizze a tűzfalat, a víruskereső szoftvert és a proxybeállításokat, és győződjön meg arról, hogy nem blokkolja az Office-alkalmazások internet-hozzáférését. Lásd [az Office 365 URL-címeket és IP-címtartományokat](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Megpróbálhatja a következő hibaelhárítási műveleteket is: 

- Nyisson meg egy Office-alkalmazást, és [Jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból. [Távolítsa el](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) , majd [rendelje hozzá ismét](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) az Office-licencet, majd [Jelentkezzen be az Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) -ba az érintett felhasználói fiókkal.
- Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Orrgazdaság a Hivatal aktiválás állapot](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Előad egy online kijavít-ból Hivatal](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

További hibaelhárítási megoldásokért lásd: 

- [Nem licencelt termék-és aktiválási hibák az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["Sajnálom, nem tudunk kapcsolódni a fiókjához. Az Office aktiválásához kérjük, próbálkozzon később.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)