---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908712"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="7ec6a-102">A BitLocker-titkosítás engedélyezése az Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="7ec6a-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="7ec6a-103">A végpontvédelmi házirendet a Windows-eszközök BitLocker titkosítási beállításainak konfigurálásához használhatja.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="7ec6a-104">További információ: [a Windows 10 (és újabb) beállításai az eszközök az Intune szolgáltatással történő védelméhez](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="7ec6a-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="7ec6a-105">Tudnia kell, hogy számos, a Windows 10 rendszert futtató újabb eszköz támogatja az automatikus BitLocker titkosítást, amely az MDM-házirend alkalmazása nélkül aktiválódik.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="7ec6a-106">Ez hatással lehet a házirendek alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="7ec6a-107">További részleteket az alábbi GYIK-ban talál.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="7ec6a-108">A BitLocker szolgáltatással kapcsolatos hibaelhárításról a [a Microsoft Intune szolgáltatás BitLocker házirendjei – problémamegoldás](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="7ec6a-109">**GYIK**</span><span class="sxs-lookup"><span data-stu-id="7ec6a-109">**FAQ**</span></span>

 <span data-ttu-id="7ec6a-110">Kérdés: a Windows mely kiadásai támogatják az eszközök titkosítását a végponti védelmi házirend segítségével?</span><span class="sxs-lookup"><span data-stu-id="7ec6a-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="7ec6a-111">A: az Intune végponti védelmi házirend beállításai a [BitLocker kriptográfiai szolgáltatójának](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)használatával vannak megvalósítva.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="7ec6a-112">Nem minden kiadás vagy Windows-Build támogatja a BitLocker kriptográfiai szolgáltatót.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="7ec6a-113">Ebben az időben a következő Windows-verziók támogatottak: Enterprise, Education, Mobile, Mobile Enterprise és Professional (Build 1809 és újabb verziók).</span><span class="sxs-lookup"><span data-stu-id="7ec6a-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="7ec6a-114">Kérdés ha egy berendezés van már encrypted-val BitLocker használ a OS hiba elintézés részére encryption módszer és rejtjel erő (XTS-AES-128), akarat alkalmaz egy politika-val különböző elintézés gépiesen ravasz ré hang-encryption-ból hajt-val a új elintézés?</span><span class="sxs-lookup"><span data-stu-id="7ec6a-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="7ec6a-115">A: nem.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-115">A: No.</span></span> <span data-ttu-id="7ec6a-116">Az új rejtjelezési beállítások alkalmazásához először a meghajtót kell dekódolt.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="7ec6a-117">**Megjegyzés:** Az automatikus vezérléssel beiratkozott eszközök esetén az OOBE során előforduló automatikus titkosítás nem kerül aktiválásra az Intune házirend kiértékelése előtt, amely lehetővé teszi a házirend alapú beállítások az operációs rendszer alapértelmezései helyett.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="7ec6a-118">Kérdés ha egy berendezés van encrypted az eredményeképpen a alkalmazás-ból Intune politika, akarat ez lenni decrypted mikor amit politika van távoli?</span><span class="sxs-lookup"><span data-stu-id="7ec6a-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="7ec6a-119">A: a titkosítással kapcsolatos házirend eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="7ec6a-120">Kérdés Miért mutat az Intune megfelelési házirend, hogy az eszközön nincs engedélyezve a BitLocker, még akkor is, ha?</span><span class="sxs-lookup"><span data-stu-id="7ec6a-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="7ec6a-121">A: az Intune megfelelési házirendben a "BitLocker engedélyezve" beállítás a Windows Eszközállapot-tanúsítvány (DHA) ügyfelének használatát használja.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="7ec6a-122">Ez az ügyfél csak az eszköz állapotát méri rendszerindításkor.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="7ec6a-123">Így ha egy eszköz nem lett újra indítva, mert a BitLocker titkosítás befejeződött, a DHA ügyfélszolgáltatás nem fogja aktívnak jelenteni a BitLocker-titkosítást.</span><span class="sxs-lookup"><span data-stu-id="7ec6a-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 