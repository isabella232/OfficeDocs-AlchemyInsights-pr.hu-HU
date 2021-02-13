---
title: A Microsoft Edge telepítése iOS, iPadOS és Android rendszeren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194521"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="57ee0-102">A Microsoft Edge telepítése iOS, iPadOS és Android rendszeren</span><span class="sxs-lookup"><span data-stu-id="57ee0-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="57ee0-103">Az alábbi interaktív forgatókönyv segítséget ad a Microsoft Edge iOS, iPadOS és Android rendszerű eszközök felhasználóihoz való hozzárendeléséhez.</span><span class="sxs-lookup"><span data-stu-id="57ee0-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="57ee0-104">Ha letiltotta a felhasználóknak a mobileszközök regisztrálását, ez az interaktív forgatókönyv nem működik, és a felhasználóknak saját telepítésük lesz a Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="57ee0-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="57ee0-105">Az interaktív forgatókönyv az alábbi lépéseket foglalja magában:</span><span class="sxs-lookup"><span data-stu-id="57ee0-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="57ee0-106">Előfeltételek</span><span class="sxs-lookup"><span data-stu-id="57ee0-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="57ee0-107">Bevezetés</span><span class="sxs-lookup"><span data-stu-id="57ee0-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="57ee0-108">Alapismeretek</span><span class="sxs-lookup"><span data-stu-id="57ee0-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="57ee0-109">Konfiguráció</span><span class="sxs-lookup"><span data-stu-id="57ee0-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="57ee0-110">Feladatok</span><span class="sxs-lookup"><span data-stu-id="57ee0-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="57ee0-111">Áttekintés és létrehozás</span><span class="sxs-lookup"><span data-stu-id="57ee0-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="57ee0-112">Az irányított forgatókönyv lépéseinek befejezése után a Microsoft Intune-házirendek engedélyezik a Microsoft Edge vállalati verziójának alábbi funkcióit:</span><span class="sxs-lookup"><span data-stu-id="57ee0-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="57ee0-113">Kettős identitás</span><span class="sxs-lookup"><span data-stu-id="57ee0-113">Dual identity</span></span>
- <span data-ttu-id="57ee0-114">Integráció a Microsoft Intune alkalmazásvédelmi szabályzatával</span><span class="sxs-lookup"><span data-stu-id="57ee0-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="57ee0-115">Integráció az Azure Active Directory alkalmazásproxyval</span><span class="sxs-lookup"><span data-stu-id="57ee0-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="57ee0-116">Felügyelt kedvencek és kezdőlap-billentyűparancsok</span><span class="sxs-lookup"><span data-stu-id="57ee0-116">Managed favorites and home page shortcuts</span></span>
