---
title: Intune-eszközleltár
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439655"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="23c82-102">Intune-eszközleltár</span><span class="sxs-lookup"><span data-stu-id="23c82-102">Intune Device Inventory</span></span>

<span data-ttu-id="23c82-103">Az Eszközök panel eszközalapon betekintést nyújt a rendszergazdai eszközökbe az Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="23c82-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="23c82-104">A megjelenített információk a következők: hardver, felderített alkalmazások, eszközmegfelelőségi állapot és eszközkonfigurációállapota.</span><span class="sxs-lookup"><span data-stu-id="23c82-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="23c82-105">A hardverek és a felderített alkalmazások készletadatait hétnapos ciklusban gyűjtik.</span><span class="sxs-lookup"><span data-stu-id="23c82-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="23c82-106">A jelentett alkalmazások és hardverelemek az eszköz operációs rendszerétől és attól függően változnak, hogy az eszköz személyes vagy vállalati tulajdonban van-e.</span><span class="sxs-lookup"><span data-stu-id="23c82-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="23c82-107">További információ: [Az eszköz részletei az Intune-ban.](https://docs.microsoft.com/intune/device-inventory)</span><span class="sxs-lookup"><span data-stu-id="23c82-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="23c82-108">**GYIK**</span><span class="sxs-lookup"><span data-stu-id="23c82-108">**FAQ**</span></span>

<span data-ttu-id="23c82-109">K: Nem kapom meg az Intune által regisztrált Windows-eszközökön található alkalmazások teljes leltárlistáját.</span><span class="sxs-lookup"><span data-stu-id="23c82-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="23c82-110">miért ne?</span><span class="sxs-lookup"><span data-stu-id="23c82-110">Why not?</span></span>

<span data-ttu-id="23c82-111">A: Jelenleg csak a vállalati eszközként azonosított Windows 10-es számítógépeken csak a modern alkalmazások jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="23c82-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="23c82-112">Az Intune nem gyűjt adatokat az ezekre az eszközökre telepített Win32-alkalmazásokról.</span><span class="sxs-lookup"><span data-stu-id="23c82-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="23c82-113">K: Miért nem gyűjtik a telefonszámokat az összes eszközről?</span><span class="sxs-lookup"><span data-stu-id="23c82-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="23c82-114">A: Az Intune-ban vállalati eszközként kategorizált telefonok nem azonosulnak a teljes telefonszámukkal, ha például mobileszköz-leltárjelentést futtat.</span><span class="sxs-lookup"><span data-stu-id="23c82-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="23c82-115">Bring-you-device telefonszámok mindig részben maszkolt csillaggal (\*\*\*\*), és csak az utolsó négy számjegy.</span><span class="sxs-lookup"><span data-stu-id="23c82-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>