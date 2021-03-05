---
title: Az AD-felhasználó kiépítési munkanapja karanténba kerül
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481876"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="78391-102">Az AD-felhasználó kiépítési munkanapja karanténba kerül</span><span class="sxs-lookup"><span data-stu-id="78391-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="78391-103">**Az AD-felhasználó kiépítési munkanapja karanténba kerül, és nem jön létre felhasználó az AD-ban**</span><span class="sxs-lookup"><span data-stu-id="78391-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="78391-104">Az AD-felhasználó kiépítési feladata karanténba került, és a naplók az exportálási hibák eseményeit mutatják a következő **hibaüzenettel: OperationsError-SvcErr: Művelethiba történt. A címtárszolgáltatáshoz nincs konfigurálva felsőbbrendű hivatkozás. A címtárszolgáltatás ezért nem tud** az erdőn kívüli objektumokra hivatkozni.</span><span class="sxs-lookup"><span data-stu-id="78391-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="78391-105">Ez a hiba általában akkor jelenik meg, ha az Active Directory-tároló szervezeti egység nincs megfelelően beállítva, vagy ha problémák vannak a **parentDistinguishedName** kifejezésleképezésével kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="78391-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="78391-106">Ellenőrizze, hogy az Új felhasználók alapértelmezett felhasználói **felhasználóinak** paramétere nem-e elkallokokat.</span><span class="sxs-lookup"><span data-stu-id="78391-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="78391-107">Győződjön meg arról, hogy a megadott szervezeti egység már szerepel az AD-ben.</span><span class="sxs-lookup"><span data-stu-id="78391-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="78391-108">Ha a **parentDistinguishedName** értéket használja az attribútumleképezésben, gondoskodjon arról, hogy az mindig egy ismert tároló legyen az AD tartományon belül.</span><span class="sxs-lookup"><span data-stu-id="78391-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="78391-109">A létrehozott érték megtekintéséhez ellenőrizze az Exportálás eseményt a naplókban.</span><span class="sxs-lookup"><span data-stu-id="78391-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="78391-110">A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további információkért lásd: A Munkanap beállítása automatikus felhasználói [kiépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="78391-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

