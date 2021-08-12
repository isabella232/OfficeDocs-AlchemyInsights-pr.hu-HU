---
title: A felhasználók kártékony e-mailt kaptak?
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929199"
---
# <a name="did-your-users-receive-malicious-email"></a>A felhasználók kártékony e-mailt kaptak?

- Mostantól bejelentheti a kártékony e-maileket a Microsoftnak a [Biztonsági és megfelelőségi központ Adminisztrátorok által beküldött elemek területén](https://sip.protection.office.com/reportsubmission).

Az [Adminisztrátorok által beküldött elemek](https://sip.protection.office.com/reportsubmission) között beküldött üzeneteket megvizsgáljuk, és az alábbi eredményeknek kell megjelenniük a **Részletek** előugró panelen:

- Történt-e hiba a küldő e-mailjének hitelesítésekor az üzenet kézbesítése során.
- Tájékoztatás azokról a házirendnek való megfelelésekről, amelyek befolyásolhatták vagy felülbírálhatták az üzenetre vonatkozó biztonsági rendelkezést.
- Az aktuális hatástalanítási eredmények, amelyekből megállapítható, hogy az üzenetben szereplő URL-címek vagy fájlok kártékonyak voltak-e, vagy sem.
- Visszajelzés az osztályozóktól

Felülbírálás esetén az újbóli vizsgálatnak néhány perc alatt be kell fejeződnie. Ha nem volt probléma az e-mail hitelesítése során, vagy ha nem befolyásolta felülbírálás a kézbesítést, az osztályozóktól kapott visszajelzésre akár egy napot is várnia kellhet.

Ha nem ért egyet egy üzenetre, URL-címre vagy fájlra vonatkozó végső biztonsági rendelkezéssel (letiltva vagy nem letiltva), egy nap múlva küldje el újra az üzenetet újbóli vizsgálatra. Az üzenet újbóli beküldése után a biztonsági rendelkezés nagy valószínűséggel megváltozik majd.

Eközben az [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) olvasható utasításokat követve eltávolíthatja a kártékony e-maileket a felhasználók postaládájából.

- Az Office 365-höz készült Microsoft Defendert használó ügyfeleknek a következőkre nyílik lehetőségük:
    - A [Veszélyforrás-felderítővel megkereshetik és törölhetik a gyanús e-maileket](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered).
    - A [Biztonságos hivatkozások funkcióval letilthatják a hozzáférést](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a kártékony URL-címekhez.
    - Nyomon követhetik a kártékony URL-címre kattintó és azt megnyitó felhasználókat: [Megtekinthetik az adathalász URL-címek és kattintási biztonsági rendelkezések adatait](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace).
    - Manuálisan [elindíthatnak egy automatizált vizsgálatot](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office).

A [Védelem a kártékony URL-címekkel és fájlokkal szemben](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) című témakörben leírt utasításokat követve is biztosíthatja a kártékony fájlokkal és URL-címekkel szembeni védelmet.