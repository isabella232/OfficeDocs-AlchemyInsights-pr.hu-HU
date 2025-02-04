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
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326673"
---
# <a name="did-your-users-receive-malicious-email"></a>A felhasználók kártékony e-mailt kaptak?

Mostantól bejelentheti a kártékony e-maileket a Microsoftnak [a Microsoft 365 Defender-portálon](https://sip.security.microsoft.com/reportsubmission?viewid=admin)keresztül.

A rendszer [beolvassa](https://security.microsoft.com/reportsubmission?viewid=admin) a rendszergazdai beküldésbe küldött üzeneteket, és a következő eredményeket mutatja a részletes elő panelen:

- Történt-e hiba a küldő e-mailjének hitelesítésekor az üzenet kézbesítése során.
- Tájékoztatás azokról a házirendnek való megfelelésekről, amelyek befolyásolhatták vagy felülbírálhatták az üzenetre vonatkozó biztonsági rendelkezést.
- Az aktuális hatástalanítási eredmények, amelyekből megállapítható, hogy az üzenetben szereplő URL-címek vagy fájlok kártékonyak voltak-e, vagy sem.
- Visszajelzés az osztályozóktól

Felülbírálás esetén az újbóli vizsgálatnak néhány perc alatt be kell fejeződnie. Ha nem volt probléma az e-mail hitelesítése során, vagy ha nem befolyásolta felülbírálás a kézbesítést, az osztályozóktól kapott visszajelzésre akár egy napot is várnia kellhet.

Ha nem ért egyet egy üzenetre, URL-címre vagy fájlra vonatkozó végső biztonsági rendelkezéssel (letiltva vagy nem letiltva), egy nap múlva küldje el újra az üzenetet újbóli vizsgálatra. Az üzenet újbóli beküldése után a biztonsági rendelkezés nagy valószínűséggel megváltozik majd.

Eközben az [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) olvasható utasításokat követve eltávolíthatja a kártékony e-maileket a felhasználók postaládájából.

- Az Office 365-höz készült Microsoft Defendert használó ügyfeleknek a következőkre nyílik lehetőségük:
  - Gyanús [e-mailek megkerese és törlése a Veszélyforrás-intézővel](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [A Széf url-hez való](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) hozzáférés blokkolása a hivatkozásokkal
  - A kártékony URL-címekre kattintó és hozzáférő felhasználók nyomon követése: Az [adathalászati URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)megtekintése és a döntési adatok betöltési-UrlTrace  &  [gombja](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Automatikus [vizsgálat kézi létrehozása](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

A [Védelem a kártékony URL-címekkel és fájlokkal szemben](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) című témakörben leírt utasításokat követve is biztosíthatja a kártékony fájlokkal és URL-címekkel szembeni védelmet.
