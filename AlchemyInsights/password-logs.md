---
title: Jelszónaplók
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525140"
---
# <a name="password-logs"></a>Jelszónaplók

**Problémákat tapasztalok a jelszó-visszaállítási naplók elérése során**

A jelszó-visszaállítási naplókhoz való hozzáféréssel kapcsolatos hibák elhárításához végezze el az alábbi lépéseket:

Győződjön meg arról, hogy jogosult a naplók megtekintésére. 

Csak az alábbi szerepkörök engedélyezettek:
 - Globális rendszergazda
 - Biztonsági rendszergazda
 - Biztonsági olvasó

**Szeretném látni az összes jelszó-visszaállítási naplóeseményt a kezdeti telepítés után**

Az elmúlt 30 nap jelentései legfeljebb 120 000 jelszó-visszaállítási/regisztrációs eseményt tárolnak. Ez a korlát a FELHASZNÁLÓI felületre vonatkozik a CSV letöltésekor. 1 millió esemény érhető el a PowerShellen keresztül.
További információt az alábbi hivatkozásokra kattintva olvashat:

- [Önkiszolgáló jelszó-visszaállítási események az Azure AD-jelentések és -események API-ból](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jelszó-visszaállítási események gyors letöltése a PowerShell használatával](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Többet szeretnék tudni a jelszó-visszaállítás jelentéskészítési lehetőségeiről**

Az Azure AD jelszó-visszaállítási naplóival ellenőrizheti, hogy kik regisztrálnak vagy állíthatnak alaphelyzetbe jelszavakat a Felhasználók és csoportok csoport Azure Portal **portálján.**
További információért lásd az alábbi hivatkozásokat:

- [Jelszó-visszaállítási jelentések áttekintése](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jelszó-visszaállítási jelentések megtekintése az Azure Portalon](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Önkiszolgáló jelszó-visszaállítási események az Azure AD-jelentések és -események API-ból](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jelszó-visszaállítási események gyors letöltése a PowerShell használatával](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


