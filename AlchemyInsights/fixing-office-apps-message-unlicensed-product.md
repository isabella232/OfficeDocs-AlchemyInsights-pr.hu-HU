---
title: Nem aktiválható az Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893913"
---
# <a name="unable-to-activate-office"></a>Nem aktiválható az Office

**Megjegyzés:** Ha a Windows régebbi verzióját használja (például Windows 7), gondoskodjon arról, hogy alapértelmezés szerint a TLS 1.2 legyen engedélyezve. További információt a Frissítés a [TLS 1.1 és a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)alapértelmezett biztonságos protokollként való engedélyezéséhez a Windowsbanhttps://Windows.

- Ellenőrizze, hogy nem járt-e le az előfizetése állapota.
- Ellenőrizze, hogy van-e olyan előfizetése, amely lehetővé teszi az ügyféllicencek használatát (például Office 365 Vállalati verzió vagy Vállalati prémium verzió), és [gondoskodjon arról, hogy a felhasználóhoz legyen hozzárendelve licenc](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Ellenőrizze, hogy a felhasználó ugyanazzal a fiókkal jelentkezik-e be az Office-ba, amelyhez a licencet hozzárendelték.
- Ellenőrizze az [Office 365 Szolgáltatásállapot lap](https://docs.microsoft.com/office365/enterprise/view-service-health) című témakört, hogy lássa, vannak-e ismert problémák a szolgáltatással kapcsolatban.
- A tűzfalat, a víruskeresőt és a proxybeállításokat ellenőrizve győződjön meg arról, hogy azok nem blokkolják a Microsoft 365-alkalmazások hozzáférését az internethez. Olvassa el [Az Office 365 URL-címei és IP-címtartományai](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Az Office 365 URL-címei és IP-címtartományai") című cikket.

**Tipp** Windows rendszerű gépeken számos gyakori Office-bejelentkezési problémát diagnosztizálhatunk és automatikusan kijavíthatunk Ön helyett. Automatizált eszközünk használatához töltse le és futtassa a **[Microsoft Támogatási és helyreállítási segédet](https://aka.ms/SaRA-OfficeSignInScenario)**.

Használja az alábbi hibaelhárítási műveleteket:

- Nyisson meg egy Office-appot, és [jelentkezzen ki](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) minden meglévő felhasználói fiókból. [Távolítsa el](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) és [rendelje újból hozzá az](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licencet, majd [jelentkezzen be az Office-ba](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) az érintett felhasználói fiókkal.
- Futtassa az [aktiválási hibaelhárítót](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Állítsa vissza az Office aktiválási állapotát](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Állítsa vissza az Office aktiválási állapotát")
- [Végezze el az Office online javítását](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

További hibaelhárítási megoldásért lásd:  

- [„Nem licencelt termék” aktiválási hibaüzenetek az Office-ban](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [A „Sajnos nem lehet csatlakozni a fiókjához. Próbálkozzon újra” hibaüzenet jelenik meg az Office aktiválásakor](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)