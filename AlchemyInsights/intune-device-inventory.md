---
title: Intune-eszköz készlete
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667880"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="2c381-102">Intune-eszköz készlete</span><span class="sxs-lookup"><span data-stu-id="2c381-102">Intune Device Inventory</span></span>

<span data-ttu-id="2c381-103">Az eszközök Blade segítségével a rendszergazda betekintést adhat az Intune-eszközökhöz eszközönként.</span><span class="sxs-lookup"><span data-stu-id="2c381-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="2c381-104">A megjelenített adatok a következők: hardver, az észlelt alkalmazások, az eszköz megfelelőségi állapota és az eszköz konfigurációja állapota.</span><span class="sxs-lookup"><span data-stu-id="2c381-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="2c381-105">A hardverek és a felfedezett alkalmazások leltározása hét napos ciklusban történik.</span><span class="sxs-lookup"><span data-stu-id="2c381-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="2c381-106">Az alkalmazások és a hardver bizonyos elemei eltérőek lehetnek az eszköz operációs rendszertől függően, és hogy az eszköz személyes vagy vállalati tulajdonú-e.</span><span class="sxs-lookup"><span data-stu-id="2c381-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="2c381-107">További információt az [eszközök adatainak megtekintése az Intune-ban](https://docs.microsoft.com/intune/device-inventory)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="2c381-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="2c381-108">**GYIK**</span><span class="sxs-lookup"><span data-stu-id="2c381-108">**FAQ**</span></span>

<span data-ttu-id="2c381-109">K: nem kapok teljes leltározási listát az Intune által regisztrált Windows-eszközökön lévő alkalmazásokról.</span><span class="sxs-lookup"><span data-stu-id="2c381-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="2c381-110">miért ne?</span><span class="sxs-lookup"><span data-stu-id="2c381-110">Why not?</span></span>

<span data-ttu-id="2c381-111">A: jelenleg csak a modern alkalmazások jelennek meg a Windows 10 rendszerű PC-ken, amelyeket vállalati eszközökként azonosítottak.</span><span class="sxs-lookup"><span data-stu-id="2c381-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="2c381-112">Az Intune nem gyűjt információkat az ilyen eszközökön telepített Win32-alkalmazásokról.</span><span class="sxs-lookup"><span data-stu-id="2c381-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="2c381-113">K.: Miért nem minden eszközről gyűjtenek telefonszámot?</span><span class="sxs-lookup"><span data-stu-id="2c381-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="2c381-114">A: az Intune-ban a vállalati eszközökként kategorizált telefonok esetében a rendszer nem azonosítja a teljes telefonszámot, ha például mobileszköz-készletezési jelentést futtat.</span><span class="sxs-lookup"><span data-stu-id="2c381-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="2c381-115">A bringa-you-Own-Phone-telefonszámokat mindig részlegesen maszkolt csillagokkal (\* \* \* \*), és csak az utolsó négy számjegyet jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="2c381-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>