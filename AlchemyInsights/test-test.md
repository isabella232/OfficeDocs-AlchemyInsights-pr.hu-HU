---
title: Hiányzó kifejezések a SharePoint Online Kifejezéstárból
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766855"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="84385-102">Bitlocker titkosítás engedélyezése az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="84385-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="84385-103">Az Intune Endpoint Protection Policy segítségével konfigurálhatja a Boitlocker titkosítási beállításait a Windows-eszközökhöz a következő részben leírtak szerint: Windows10 (és újabb) beállítások az Eszközök Intune-t használó védelmére</span><span class="sxs-lookup"><span data-stu-id="84385-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="84385-104">Tudnia kell, hogy sok újabb, Windows 10-et futtató eszköz támogatja az automatikus bitlocker titkosítást, amely az MDM-házirend alkalmazása nélkül aktiválódik.</span><span class="sxs-lookup"><span data-stu-id="84385-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="84385-105">Ez hatással lehet a házirend alkalmazására, ha nem alapértelmezett beállítások vannak konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="84385-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="84385-106">További részletekért lásd a GYIK-et.</span><span class="sxs-lookup"><span data-stu-id="84385-106">See FAQ for more detail.</span></span>


<span data-ttu-id="84385-107">Gyakran  feltett kérdések: A Windows mely kiadásai támogatják az eszköztitkosítást a Végpontvédelmi szabályzat használatával?</span><span class="sxs-lookup"><span data-stu-id="84385-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="84385-108"> A: Az Intune Végpontvédelmi házirend beállításai a Bitlocker csp használatával vannak megvalósítva.</span><span class="sxs-lookup"><span data-stu-id="84385-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="84385-109">Nem minden windowsos kiadás és build támogatja a Bitlocker csp-t. 
     </span><span class="sxs-lookup"><span data-stu-id="84385-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="84385-110">Jelenleg windows os kiadások: Enterprise; Az oktatás, a mobil, a mobil vállalkozás és a profi (a build 1809-től) támogatottak.</span><span class="sxs-lookup"><span data-stu-id="84385-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="84385-111">K: Ha egy eszköz már titkosítva Bitlocker segítségével az operációs rendszer alapértelmezett beállításait titkosítási módszer és a titkosítás erőssége (XTS-AES-128) fogja alkalmazni a politika különböző beállításokkal automatikusan elindítja újratitkosítása a meghajtó az új beállításokat?</span><span class="sxs-lookup"><span data-stu-id="84385-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="84385-112">A: Nem.</span><span class="sxs-lookup"><span data-stu-id="84385-112">A: No.</span></span> <span data-ttu-id="84385-113">Az új titkosítási beállítások alkalmazásához a meghajtót először vissza kell fejteni.</span><span class="sxs-lookup"><span data-stu-id="84385-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="84385-114">Megjegyzés: Az Autopilot szolgáltatással regisztrált eszközök esetében az OOBE során fellépő automatikus titkosítás csak az Intune-házirend kiértékelése után aktiválódik, amely lehetővé teszi, hogy a házirend-alapú beállításokat az operációs rendszer alapértelmezései helyett használják.</span><span class="sxs-lookup"><span data-stu-id="84385-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="84385-115">K Ha egy eszköz titkosítva van az Intune-házirend alkalmazása miatt, visszafejti a rendszer a házirend eltávolításakor?</span><span class="sxs-lookup"><span data-stu-id="84385-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="84385-116">A: A titkosítással kapcsolatos házirend eltávolítása NEM eredményezi a konfigurált meghajtók visszafejtését.</span><span class="sxs-lookup"><span data-stu-id="84385-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="84385-117">K: Miért mutatja az Intune megfelelőségi szabályzata, hogy az eszközömnem rendelkezik "Bitlocker engedélyezve", de az igen?</span><span class="sxs-lookup"><span data-stu-id="84385-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="84385-118">Megjegyzés: Az Intune megfelelőségi házirendjének "Bitlocker-engedélyezése" beállítása a Windows eszközállapot-igazolási (DHA) ügyfelet használja.</span><span class="sxs-lookup"><span data-stu-id="84385-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="84385-119">Ez az ügyfél csak a rendszerindításkor méri az eszköz állapotát.</span><span class="sxs-lookup"><span data-stu-id="84385-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="84385-120">Tehát ha egy eszköz nem lett újraindítva a bitlocker titkosítás befejezése óta, a DHA ügyfélszolgáltatás nem jelenti a bitlocker aktívként való jelentését.</span><span class="sxs-lookup"><span data-stu-id="84385-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>