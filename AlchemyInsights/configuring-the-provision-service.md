---
title: A Provision szolgáltatás konfigurálása
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482869"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="79827-102">A Provision szolgáltatás konfigurálása</span><span class="sxs-lookup"><span data-stu-id="79827-102">Configuring the Provision service</span></span>

<span data-ttu-id="79827-103">A felhasználók automatikus kiépítése csak akkor működik, ha az Azure AD érvényes hitelesítő adatokkal rendelkezik, amelyek lehetővé teszik, hogy csatlakozzon a Workday Web Services API-hoz.</span><span class="sxs-lookup"><span data-stu-id="79827-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="79827-104">A Workday to AD User Provisioning app Tesztkapcsolat gombja ezenkívül ellenőrzi, hogy képes-e csatlakozni az AD-tartományhoz társított Azure AD Connect Provisioning Agent szolgáltatáshoz.</span><span class="sxs-lookup"><span data-stu-id="79827-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="79827-105">Ha az Azure Portal hibaüzenetet ad vissza a hitelesítő adatok mentésekor, kövesse az alábbi ajánlott lépéseket:</span><span class="sxs-lookup"><span data-stu-id="79827-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="79827-106">Ellenőrizze, hogy konfigurálta-e a Workday Integration System felhasználói fiókját a Workday alkalmazás integrációs rendszerének felhasználóit ismertető oktatóanyag [szakaszának megfelelően.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="79827-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="79827-107">Győződjön meg arról, hogy az Azure AD Connect Provisioning Agent szolgáltatás a szolgáltatások felügyeleti konzolját használva működik a helyszíni Windows-kiszolgálón.</span><span class="sxs-lookup"><span data-stu-id="79827-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="79827-108">Az Azure Portalon az ügynök állapotát a Helyszíni ügynökök megtekintése gombra kattintva is ellenőrizheti.</span><span class="sxs-lookup"><span data-stu-id="79827-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="79827-109">Győződjön meg arról, hogy a "Workday Username" mező értékét az username@workday-tenant-name formátumban adja meg.</span><span class="sxs-lookup"><span data-stu-id="79827-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="79827-110">Ha a munkanap-bérlő-név hiányzik, a Workday-hitelesítés sikertelen lesz.</span><span class="sxs-lookup"><span data-stu-id="79827-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="79827-111">Ha a Workday implementációs bérlői fiókkal konfigurálja az integrációt, jegyezze fel a Workday-bérlő ütemezett állásidejét.</span><span class="sxs-lookup"><span data-stu-id="79827-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="79827-112">A munkabeosztási bérlők leállását a hétvégékre (általában péntek estétől szombat reggelig) ütemezte, és a leállási időkeret csatlakozási sikertelenségei ismert problémát jelentek, amely automatikusan megoldja a problémát, amint a bérlők újra online állapotba állnak.</span><span class="sxs-lookup"><span data-stu-id="79827-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="79827-113">Ritkán ez a hibaüzenet akkor is előfordulhat, ha az integrálórendszer-felhasználó jelszava megváltozott a bérlői fiók frissítése miatt, vagy ha a fiók zárolt vagy lejárt állapotban van.</span><span class="sxs-lookup"><span data-stu-id="79827-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="79827-114">Ellenőrizze az integrációs rendszer felhasználójának állapotát a Workday rendszergazdájával.</span><span class="sxs-lookup"><span data-stu-id="79827-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="79827-115">A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további információkért lásd: A Munkanap beállítása automatikus felhasználói [kiépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="79827-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
