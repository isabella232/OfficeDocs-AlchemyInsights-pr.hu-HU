---
title: Nem lehet aktiválni az Office-t
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: ee4618bd288e3e8be75dc969af58f921a14f48b0
ms.sourcegitcommit: bf87d91fa60bd961bc6c887c4a4be7a3c7665b38
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44474499"
---
# <a name="unable-to-activate-office"></a>Nem lehet aktiválni az Office-t

- Ellenőrizze, hogy nem járt-e le az előfizetése állapota.
- Győződjön meg arról, hogy olyan előfizetéssel rendelkezik, amely lehetővé teszi az ügyféllicencek, például az Office 365 Vállalati verzió vagy a Vállalati prémium verzió előfizetését, és [győződjön meg arról, hogy a felhasználóhoz licenc van hozzárendelve.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users)
- Ellenőrizze, hogy a felhasználó ugyanazzal a fiókkal jelentkezik-e be az Office-ba, amelyhez a licencet hozzárendelték.
- Ellenőrizze az [Office 365 Szolgáltatásállapot lap](https://docs.microsoft.com/office365/enterprise/view-service-health) című témakört, hogy lássa, vannak-e ismert problémák a szolgáltatással kapcsolatban.
- A tűzfalat, a víruskeresőt és a proxybeállításokat ellenőrizve győződjön meg arról, hogy azok nem blokkolják az Office-appok hozzáférését az internethez. Olvassa el [Az Office 365 URL-címei és IP-címtartományai](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "Az Office 365 URL-címei és IP-címtartományai") című cikket.

Használja az alábbi hibaelhárítási műveleteket:

- Nyisson meg egy Office-appot, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból. [Távolítsa el](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Eltávolít") és [rendelje újból hozzá az](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "újrahozzárendelés") Office-licencet, majd [jelentkezzen be az Office-ba](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "bejelentkezés az Office-ba") az érintett felhasználói fiókkal.
- Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/en-us/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office aktiválási állapotának alaphelyzetbe állítása")
- [Végezze el az Office online javítását](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

További hibaelhárítási megoldásért lásd:  
[„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
["Sajnáljuk, nem tudunk csatlakozni a fiókjához. Kérjük, próbálkozzon később" hibaüzenet az Office aktiválásakor]( https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 ""Sajnáljuk, nem tudunk csatlakozni a fiókjához. Kérjük, próbálja meg később" hibaüzenet az Office aktiválásakor")