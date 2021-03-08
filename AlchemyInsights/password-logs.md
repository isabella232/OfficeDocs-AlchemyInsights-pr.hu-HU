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
# <a name="password-logs"></a><span data-ttu-id="ef238-102">Jelszónaplók</span><span class="sxs-lookup"><span data-stu-id="ef238-102">Password logs</span></span>

<span data-ttu-id="ef238-103">**Problémákat tapasztalok a jelszó-visszaállítási naplók elérése során**</span><span class="sxs-lookup"><span data-stu-id="ef238-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="ef238-104">A jelszó-visszaállítási naplókhoz való hozzáféréssel kapcsolatos hibák elhárításához végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="ef238-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="ef238-105">Győződjön meg arról, hogy jogosult a naplók megtekintésére.</span><span class="sxs-lookup"><span data-stu-id="ef238-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="ef238-106">Csak az alábbi szerepkörök engedélyezettek:</span><span class="sxs-lookup"><span data-stu-id="ef238-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="ef238-107">Globális rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ef238-107">Global administrator</span></span>
 - <span data-ttu-id="ef238-108">Biztonsági rendszergazda</span><span class="sxs-lookup"><span data-stu-id="ef238-108">Security administrator</span></span>
 - <span data-ttu-id="ef238-109">Biztonsági olvasó</span><span class="sxs-lookup"><span data-stu-id="ef238-109">Security reader</span></span>

<span data-ttu-id="ef238-110">**Szeretném látni az összes jelszó-visszaállítási naplóeseményt a kezdeti telepítés után**</span><span class="sxs-lookup"><span data-stu-id="ef238-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="ef238-111">Az elmúlt 30 nap jelentései legfeljebb 120 000 jelszó-visszaállítási/regisztrációs eseményt tárolnak.</span><span class="sxs-lookup"><span data-stu-id="ef238-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="ef238-112">Ez a korlát a FELHASZNÁLÓI felületre vonatkozik a CSV letöltésekor.</span><span class="sxs-lookup"><span data-stu-id="ef238-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="ef238-113">1 millió esemény érhető el a PowerShellen keresztül.</span><span class="sxs-lookup"><span data-stu-id="ef238-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="ef238-114">További információt az alábbi hivatkozásokra kattintva olvashat:</span><span class="sxs-lookup"><span data-stu-id="ef238-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="ef238-115">Önkiszolgáló jelszó-visszaállítási események az Azure AD-jelentések és -események API-ból</span><span class="sxs-lookup"><span data-stu-id="ef238-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ef238-116">Jelszó-visszaállítási események gyors letöltése a PowerShell használatával</span><span class="sxs-lookup"><span data-stu-id="ef238-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="ef238-117">**Többet szeretnék tudni a jelszó-visszaállítás jelentéskészítési lehetőségeiről**</span><span class="sxs-lookup"><span data-stu-id="ef238-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="ef238-118">Az Azure AD jelszó-visszaállítási naplóival ellenőrizheti, hogy kik regisztrálnak vagy állíthatnak alaphelyzetbe jelszavakat a Felhasználók és csoportok csoport Azure Portal **portálján.**</span><span class="sxs-lookup"><span data-stu-id="ef238-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="ef238-119">További információért lásd az alábbi hivatkozásokat:</span><span class="sxs-lookup"><span data-stu-id="ef238-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="ef238-120">Jelszó-visszaállítási jelentések áttekintése</span><span class="sxs-lookup"><span data-stu-id="ef238-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ef238-121">Jelszó-visszaállítási jelentések megtekintése az Azure Portalon</span><span class="sxs-lookup"><span data-stu-id="ef238-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ef238-122">Önkiszolgáló jelszó-visszaállítási események az Azure AD-jelentések és -események API-ból</span><span class="sxs-lookup"><span data-stu-id="ef238-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="ef238-123">Jelszó-visszaállítási események gyors letöltése a PowerShell használatával</span><span class="sxs-lookup"><span data-stu-id="ef238-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


