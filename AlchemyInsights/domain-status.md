---
title: Domain Status (Tartomány állapota) – Nincs kijelölt szolgáltatás
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1476a88c7b974a9e6cfe443f6842df8cdc3d7073a73c0add7e6f183dd0528de1
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874397"
---
# <a name="domain-status---no-services-selected"></a>Domain Status (Tartomány állapota) – Nincs kijelölt szolgáltatás

**Nincs kijelölt** szolgáltatás, az azt jelenti, hogy még nem jelölt ki Microsoft 365-szolgáltatásokat (például Exchange Online, Skype Vállalati verzió vagy Intune, illetve Microsoft 365 mobileszköz-kezelés az egyéni tartománnyal való használatra). Ha hibrid (helyszíni Exchange Exchange Exchange Online-val) vagy külső levélszemétszűrésben használja az Exchange-t , és más Microsoft-szolgáltatások, figyelmen kívül hagyhatja ezt az üzenetet. A tartomány állapota csak a közvetlenül a szolgáltatáshoz csatlakoztatott tartományokhoz érhető el.

Szolgáltatások kiválasztása a tartományhoz:

1. A **Gépház** tartományok csoportban jelölje be a tartomány melletti jelölőnégyzetet a Nincs kijelölt szolgáltatások  >  [](https://admin.microsoft.com/Adminportal/Home) **állapotüzenettel.**
1. A **Dns kezelése lehetőséget** választva indítsa el a Tartománybeállítási varázslót.
    - Ha a **Saját DNS-rekordok hozzáadása lehetőséget választja,** amikor a rendszer kéri, válasszon egy szolgáltatást. További szolgáltatások a Speciális beállítások **alatt érhetők el.**
    - Ha A **Microsoft hozzáadhatja** a DNS-rekordjait vagy a További beállítások beállítását választja, a rendszer automatikusan javasolja és kiválasztja az  >  **online** szolgáltatásokat.
1. Folytassa a varázsló lépéseit a DNS beállításának és a szolgáltatásbeállításoknak a befejezéséhez.
 
A tartomány beállításával kapcsolatos további segítségért lásd: [A tartomány csatlakoztatása DNS-rekordok hozzáadása.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

