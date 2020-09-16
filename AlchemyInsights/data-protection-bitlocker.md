---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731241"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="483f3-102">A BitLocker-titkosítás engedélyezése a Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="483f3-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="483f3-103">A Intune végpont-védelmi házirend segítségével konfigurálhatók a Windows-eszközök BitLocker-titkosítási beállításai.</span><span class="sxs-lookup"><span data-stu-id="483f3-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="483f3-104">További információt a [Windows 10 (vagy újabb verzió) beállításai](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)című témakörben talál a Intune segítségével.</span><span class="sxs-lookup"><span data-stu-id="483f3-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="483f3-105">Felhívjuk a figyelmét arra, hogy a Windows 10 rendszert futtató számos újabb eszköz támogatja az automatikus BitLocker-titkosítást, amelyet a MDM házirend alkalmazása nélkül indítanak el.</span><span class="sxs-lookup"><span data-stu-id="483f3-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="483f3-106">Ez hatással lehet a házirend alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="483f3-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="483f3-107">További részleteket az alábbi gyakori kérdések című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="483f3-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="483f3-108">A BitLocker-problémák elhárításáról a [BitLocker-házirendek hibaelhárítása a Microsoft Intune-ban](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="483f3-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="483f3-109">**GYIK**</span><span class="sxs-lookup"><span data-stu-id="483f3-109">**FAQ**</span></span>

 <span data-ttu-id="483f3-110">K.: a Windows mely kiadásai támogatják az eszközök titkosítását a Endpoint Protection Policy?</span><span class="sxs-lookup"><span data-stu-id="483f3-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="483f3-111">A: az Intune végpontok védelmi házirendjének beállításai a [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)segítségével valósulnak meg.</span><span class="sxs-lookup"><span data-stu-id="483f3-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="483f3-112">Nem minden Windows-kiadás vagy-Build támogatja a BitLocker CSP-t.</span><span class="sxs-lookup"><span data-stu-id="483f3-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="483f3-113">Jelenleg a következő Windows-kiadások támogatottak: nagyvállalati, oktatási, mobil, mobil Enterprise és Professional (1809-es vagy újabb verzió).</span><span class="sxs-lookup"><span data-stu-id="483f3-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="483f3-114">K: Ha egy eszköz már titkosított az operációs rendszer alapértelmezett titkosítási és titkosítási erősségi beállításaival (XTS-AES-128), az új beállításokkal automatikusan inicializálja a meghajtót az új beállításokkal.</span><span class="sxs-lookup"><span data-stu-id="483f3-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="483f3-115">V: Nem.</span><span class="sxs-lookup"><span data-stu-id="483f3-115">A: No.</span></span> <span data-ttu-id="483f3-116">Az új titkosítási beállítások alkalmazásához a meghajtót először vissza kell fejteni.</span><span class="sxs-lookup"><span data-stu-id="483f3-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="483f3-117">**Megjegyzés:** Az automatikus előfizetéssel regisztrált eszközök esetén az OOBE során az automatikus titkosítás nem indul el, amíg a Intune-házirend kiértékelése nem történik meg, amely lehetővé teszi, hogy az operációs rendszer alapértelmezett beállításainak helyén a házirend-alapú beállítások használhatók legyenek.</span><span class="sxs-lookup"><span data-stu-id="483f3-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="483f3-118">K: Ha az eszköz az Intune-házirend alkalmazása következtében titkosítva van, akkor a rendszer a házirend eltávolítását követően dekódolja?</span><span class="sxs-lookup"><span data-stu-id="483f3-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="483f3-119">A: a titkosítással kapcsolatos házirendek eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.</span><span class="sxs-lookup"><span data-stu-id="483f3-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="483f3-120">K.: Miért jelzi, hogy az Intune megfelelőségi házirend azt mutatja, hogy az eszközön nincs engedélyezve a BitLocker, még akkor is, ha?</span><span class="sxs-lookup"><span data-stu-id="483f3-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="483f3-121">A: a "BitLocker enabled" beállítás a Intune megfelelőségi házirendjében a Windows-eszközök állapottanúsítvány-ügyfelét használja.</span><span class="sxs-lookup"><span data-stu-id="483f3-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="483f3-122">Ez az ügyfél csak a rendszerindítás során méri az eszköz állapotát.</span><span class="sxs-lookup"><span data-stu-id="483f3-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="483f3-123">Így ha egy eszköz nem lett újraindítva, mert a BitLocker-titkosítás befejeződött, a DHA Client szolgáltatás nem jelenti azt, hogy a BitLocker aktív marad.</span><span class="sxs-lookup"><span data-stu-id="483f3-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 