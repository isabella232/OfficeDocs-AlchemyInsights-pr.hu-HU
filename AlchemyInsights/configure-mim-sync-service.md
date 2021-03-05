---
title: A MIM-szinkronizálási szolgáltatás konfigurálása
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481873"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="d7e05-102">A MIM-szinkronizálási szolgáltatás konfigurálása</span><span class="sxs-lookup"><span data-stu-id="d7e05-102">Configure MIM Sync service</span></span>

<span data-ttu-id="d7e05-103">A Microsoft Identity Manager (MIM) szinkronizálási szolgáltatás a MIM összetevője.</span><span class="sxs-lookup"><span data-stu-id="d7e05-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="d7e05-104">Ez egy központosított helyszíni szolgáltatás, amely információkat tárol és integrál a több helyszíni könyvtárakkal és adatbázisokkal rendelkező szervezetek számára.</span><span class="sxs-lookup"><span data-stu-id="d7e05-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="d7e05-105">A MIM-szinkronizálással kapcsolatos problémát akkor lehet megoldani, ha a problémát egy nemrég frissülő mim-frissítésben javította, vagy ha az alábbi szakaszban említett egyéb problémák egyike.</span><span class="sxs-lookup"><span data-stu-id="d7e05-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="d7e05-106">**Ajánlott lépések**</span><span class="sxs-lookup"><span data-stu-id="d7e05-106">**Recommended steps**</span></span>

1. <span data-ttu-id="d7e05-107">Győződjön meg arról, hogy a MIM Sync legújabb frissítését használja, és ellenőrizze a [MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) kibocsátási megjegyzéseit annak megállapításához, hogy a probléma megoldódott-e egy frissítésben.</span><span class="sxs-lookup"><span data-stu-id="d7e05-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="d7e05-108">Ha a probléma az Általános LDAP, az Generic SQL, a Lotus Domino vagy a Web Services összekötővel kapcsolatos, győződjön meg arról, hogy az általános összekötők legújabb frissítését [használja.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="d7e05-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="d7e05-109">Ha egy MIM-szinkronizálási futtatása hibát jelez, [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) a lehetséges okok meghatározásához tekintse meg a futtatás hibakódokat táblázatát.</span><span class="sxs-lookup"><span data-stu-id="d7e05-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="d7e05-110">Ha a futtatás a **extension-dll-exception** kiterjesztéssel leáll, akkor a szavakra kattintva nyissa meg az **Összekötő** térobjektum tulajdonságablakát, és kattintson a Stack Trace **gombra,** hogy további információt látsson a mögöttes okról, az [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)leírásának megfelelő módon.</span><span class="sxs-lookup"><span data-stu-id="d7e05-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="d7e05-111">Ha a PCNS összetevő a **6025-ös** hibát jelenti az eseménynaplóban a jelszó-szinkronizálás során, az útmutatóban ellenőrizheti a [PCNS 6025-ös](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)hibajelentési hibáinak elhárítását.</span><span class="sxs-lookup"><span data-stu-id="d7e05-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="d7e05-112">Ha lassú a teljes szinkronizálás a FIM  szolgáltatáskezelő ügynökkel, ellenőrizze a TempDB automatikus növekvő beállítását, a lassú szinkronizálás vagy a teljes szinkronizálás lelassulása – hibaelhárítási [leírásnak megfelelő módon.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)</span><span class="sxs-lookup"><span data-stu-id="d7e05-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="d7e05-113">Ha a FIM szolgáltatáskezelő ügynökével sikertelen létrehozású webszolgáltatások esetén a leállított kiszolgáló hibát talál, az okokat áttekintheti a támogatási információk [között:](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) sikertelen létrehozás-létrehozás webszolgáltatásokon keresztül.</span><span class="sxs-lookup"><span data-stu-id="d7e05-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

