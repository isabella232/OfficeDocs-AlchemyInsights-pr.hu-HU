---
title: A SharePoint Online Kifejezéstárolóból hiányzó feltételek
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053515"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="bb589-102">A BitLocker-titkosítás engedélyezése az Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="bb589-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="bb589-103">Az Intune végpont-védelmi házirend a Windows-eszközök Boitlocker-titkosítási beállításainak az alábbiakban leírt módon történő konfigurálására használható: Windows10 (és újabb) beállítások az eszközök védelmére az Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="bb589-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="bb589-104">Tisztában kell lennie azzal, hogy sok újabb Windows 10-es rendszerű eszköz támogatja az automatikus BitLocker titkosítást, ami az MDM-házirend alkalmazása nélkül aktiválódik.</span><span class="sxs-lookup"><span data-stu-id="bb589-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="bb589-105">Ez hatással lehet a házirendek alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="bb589-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="bb589-106">További részleteket a GYIK-ban találhat.</span><span class="sxs-lookup"><span data-stu-id="bb589-106">See FAQ for more detail.</span></span>


<span data-ttu-id="bb589-107">FAQ  Q: a rendszer mely kiadásai támogatják az eszközök titkosítását a végponti védelmi házirend segítségével?</span><span class="sxs-lookup"><span data-stu-id="bb589-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="bb589-108"> A: az Intune végponti védelmi házirend beállításai a BitLocker kriptográfiai szolgáltatójának használatával vannak megvalósítva.</span><span class="sxs-lookup"><span data-stu-id="bb589-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="bb589-109">Nem minden kiadás, sem a Windows rendszer nem támogatja a BitLocker kriptográfiai szolgáltatót. 
     </span><span class="sxs-lookup"><span data-stu-id="bb589-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="bb589-110">Ebben az időben a Windows Editions: Enterprise; Oktatás, mozgatható, mozgatható vállalat és profi (-ból épít 1809 elõre) van támogatott.</span><span class="sxs-lookup"><span data-stu-id="bb589-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="bb589-111">Kérdés ha egy berendezés van már encrypted-val BitLocker használ a OS hiba elintézés részére encryption módszer és rejtjel erő (XTS-AES-128) akarat alkalmaz egy politika-val különböző elintézés gépiesen ravasz ré hang-encryption-ból hajt-val a új elintézés?</span><span class="sxs-lookup"><span data-stu-id="bb589-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="bb589-112">A: nem.</span><span class="sxs-lookup"><span data-stu-id="bb589-112">A: No.</span></span> <span data-ttu-id="bb589-113">Az új rejtjelezési beállítások alkalmazásához a meghajtónak először dekódolt kell lennie.</span><span class="sxs-lookup"><span data-stu-id="bb589-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="bb589-114">Megjegyzés: az automatikus vezérléssel beiratkozott eszközök esetében a rendszer nem indítja el az automatikus titkosítást, amíg az Intune házirend nem lesz kiértékelve, amely lehetővé teszi a házirend-alapú beállítások használtát az operációsrendszer-Alapértelmezések helyett</span><span class="sxs-lookup"><span data-stu-id="bb589-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="bb589-115">Q ha egy eszköz az Intune-házirend alkalmazása miatt titkosított, akkor a rendszer visszafejtette az adott házirend eltávolításakor?</span><span class="sxs-lookup"><span data-stu-id="bb589-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="bb589-116">A: a titkosítással kapcsolatos házirendek eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.</span><span class="sxs-lookup"><span data-stu-id="bb589-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="bb589-117">K: Miért jelenik meg az Intune megfelelési házirend, hogy az eszközön nincs "BitLocker enabled", de?</span><span class="sxs-lookup"><span data-stu-id="bb589-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="bb589-118">A: az Intune-megfelelőségi házirend "BitLocker-védelemmel ellátott" beállítása a Windows Eszközállapot-tanúsítási (DHA) ügyfelet használja.</span><span class="sxs-lookup"><span data-stu-id="bb589-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="bb589-119">Ez az ügyfél csak az eszköz állapotát méri rendszerindításkor.</span><span class="sxs-lookup"><span data-stu-id="bb589-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="bb589-120">Így ha egy eszköz nem lett újra indítva, mert a BitLocker titkosítás befejeződött, a DHA ügyfélszolgáltatás nem fogja aktívnak jelenteni a BitLocker-titkosítást.</span><span class="sxs-lookup"><span data-stu-id="bb589-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>