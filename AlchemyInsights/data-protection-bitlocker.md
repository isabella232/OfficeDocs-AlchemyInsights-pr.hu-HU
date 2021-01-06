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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768819"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="54f1a-102">A BitLocker-titkosítás engedélyezése a Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="54f1a-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="54f1a-103">A Intune végpont-védelmi házirend segítségével konfigurálhatók a Windows-eszközök BitLocker-titkosítási beállításai.</span><span class="sxs-lookup"><span data-stu-id="54f1a-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="54f1a-104">További információt a [Windows 10 (vagy újabb verzió) beállításai](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)című témakörben talál a Intune segítségével.</span><span class="sxs-lookup"><span data-stu-id="54f1a-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="54f1a-105">Felhívjuk a figyelmét arra, hogy a Windows 10 rendszert futtató számos újabb eszköz támogatja az automatikus BitLocker-titkosítást, amelyet a MDM házirend alkalmazása nélkül indítanak el.</span><span class="sxs-lookup"><span data-stu-id="54f1a-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="54f1a-106">Ez hatással lehet a házirend alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="54f1a-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="54f1a-107">További részleteket az alábbi gyakori kérdések című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="54f1a-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="54f1a-108">A BitLocker-problémák elhárításáról a [BitLocker-házirendek hibaelhárítása a Microsoft Intune-ban](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="54f1a-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="54f1a-109">**GYIK**</span><span class="sxs-lookup"><span data-stu-id="54f1a-109">**FAQ**</span></span>

<span data-ttu-id="54f1a-110">K.: a Windows mely kiadásai támogatják az eszközök titkosítását a Endpoint Protection Policy?</span><span class="sxs-lookup"><span data-stu-id="54f1a-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="54f1a-111">A: az Intune végpontok védelmi házirendjének beállításai a [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)segítségével valósulnak meg.</span><span class="sxs-lookup"><span data-stu-id="54f1a-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="54f1a-112">Nem minden Windows-kiadás vagy-Build támogatja a BitLocker CSP-t.</span><span class="sxs-lookup"><span data-stu-id="54f1a-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="54f1a-113">K.: Hogyan engedélyezhetők a BitLocker az eszközökön a végfelhasználói interakció megkövetelése nélkül?</span><span class="sxs-lookup"><span data-stu-id="54f1a-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="54f1a-114">A: a szükséges előfeltételek teljesülése esetén előfordulhat, hogy a BitLocker "Silent Encryption" funkcióját a Intune segítségével is engedélyezzük.</span><span class="sxs-lookup"><span data-stu-id="54f1a-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="54f1a-115">Az eszközök követelményeiről és a példa házirend-beállításokról a csendes titkosítás engedélyezése a következő dokumentumokban című témakörben talál további információt: a [BitLocker-titkosítás](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)engedélyezése.</span><span class="sxs-lookup"><span data-stu-id="54f1a-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="54f1a-116">K: Ha egy eszköz már titkosított az operációs rendszer alapértelmezett titkosítási és titkosítási erősségi beállításaival (XTS-AES-128), az új beállításokkal automatikusan inicializálja a meghajtót az új beállításokkal.</span><span class="sxs-lookup"><span data-stu-id="54f1a-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="54f1a-117">V: Nem.</span><span class="sxs-lookup"><span data-stu-id="54f1a-117">A: No.</span></span> <span data-ttu-id="54f1a-118">Az új titkosítási beállítások alkalmazásához a meghajtót először vissza kell fejteni.</span><span class="sxs-lookup"><span data-stu-id="54f1a-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="54f1a-119">**Megjegyzés:** Az automatikus előfizetéssel regisztrált eszközök esetén az OOBE során az automatikus titkosítás nem indul el, amíg a Intune-házirend kiértékelése nem történik meg, amely lehetővé teszi, hogy az operációs rendszer alapértelmezett beállításainak helyén a házirend-alapú beállítások használhatók legyenek.</span><span class="sxs-lookup"><span data-stu-id="54f1a-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="54f1a-120">K: Ha az eszköz az Intune-házirend alkalmazása következtében titkosítva van, akkor a rendszer a házirend eltávolítását követően dekódolja?</span><span class="sxs-lookup"><span data-stu-id="54f1a-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="54f1a-121">A: a titkosítással kapcsolatos házirendek eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.</span><span class="sxs-lookup"><span data-stu-id="54f1a-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="54f1a-122">K.: Miért jelzi, hogy az Intune megfelelőségi házirend azt mutatja, hogy az eszközön nincs engedélyezve a BitLocker, még akkor is, ha?</span><span class="sxs-lookup"><span data-stu-id="54f1a-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="54f1a-123">A: a "BitLocker enabled" beállítás a Intune megfelelőségi házirendjében a Windows-eszközök állapottanúsítvány-ügyfelét használja.</span><span class="sxs-lookup"><span data-stu-id="54f1a-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="54f1a-124">Ez az ügyfél csak a rendszerindítás során méri az eszköz állapotát.</span><span class="sxs-lookup"><span data-stu-id="54f1a-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="54f1a-125">Így ha egy eszköz nem lett újraindítva, mert a BitLocker-titkosítás befejeződött, a DHA Client szolgáltatás nem jelenti azt, hogy a BitLocker aktív marad.</span><span class="sxs-lookup"><span data-stu-id="54f1a-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 