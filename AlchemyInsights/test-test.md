---
title: A SharePoint Online term Store-ból hiányzó kifejezések
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750453"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="80df0-102">A BitLocker-titkosítás engedélyezése a Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="80df0-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="80df0-103">A Intune Endpoint Protection Policy a Windows-eszközök Boitlocker-titkosítási beállításainak konfigurálására szolgál a következő témakörben ismertetett módon: billentyűzettel történő navigáció (vagy újabb) beállítások a Intune segítségével az eszközök védelméhez</span><span class="sxs-lookup"><span data-stu-id="80df0-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="80df0-104">Felhívjuk a figyelmét arra, hogy a Windows 10 rendszert futtató számos újabb eszköz támogatja az automatikus BitLocker-titkosítást, amelyet a MDM-házirend alkalmazása nélkül indítanak el.</span><span class="sxs-lookup"><span data-stu-id="80df0-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="80df0-105">Ez hatással lehet a házirend alkalmazására, ha a nem alapértelmezett beállítások vannak konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="80df0-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="80df0-106">További részletekért olvassa el a gyakori kérdések című témakört.</span><span class="sxs-lookup"><span data-stu-id="80df0-106">See FAQ for more detail.</span></span>


<span data-ttu-id="80df0-107">Gyakori kérdések   : a Windows mely kiadásai támogatják az eszközök titkosítását a Endpoint Protection Policy segítségével?</span><span class="sxs-lookup"><span data-stu-id="80df0-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="80df0-108"> A: az Intune végpontok védelmi házirendjének beállításai a BitLocker CSP segítségével valósulnak meg.</span><span class="sxs-lookup"><span data-stu-id="80df0-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="80df0-109">Nem minden kiadás és a Windows buildei támogatják a BitLocker CSP-t. 
     </span><span class="sxs-lookup"><span data-stu-id="80df0-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="80df0-110">Jelenleg a Windows kiadás: Enterprise; Az oktatás, a mobil, a mobil Enterprise és a Professional (az 1809-től kezdődően) támogatott.</span><span class="sxs-lookup"><span data-stu-id="80df0-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="80df0-111">K: Ha egy eszköz már titkosítva van a BitLocker alkalmazással a titkosítási mód alapértelmezett beállításaival (XTS-AES-128) egy olyan házirendet fog alkalmazni, amelyben az új beállítások automatikusan kikapcsolják a meghajtó ismételt titkosítását?</span><span class="sxs-lookup"><span data-stu-id="80df0-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="80df0-112">V: Nem.</span><span class="sxs-lookup"><span data-stu-id="80df0-112">A: No.</span></span> <span data-ttu-id="80df0-113">Az új titkosítási beállítások alkalmazása érdekében a meghajtót először vissza kell fejteni.</span><span class="sxs-lookup"><span data-stu-id="80df0-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="80df0-114">Megjegyzés: az automatikus előfizetéssel regisztrált eszközök esetén az OOBE során bekövetkezett automatikus titkosítás nem indul el, amíg a Intune-házirend kiértékelése megtörténik, amely lehetővé teszi az operációs rendszer alapértelmezett beállításainak helyén a házirend-alapú beállítások használatát.</span><span class="sxs-lookup"><span data-stu-id="80df0-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="80df0-115">K: Ha egy eszköz az Intune-házirend alkalmazása következtében titkosítva van, akkor a rendszer a házirend eltávolítását követően dekódolja?</span><span class="sxs-lookup"><span data-stu-id="80df0-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="80df0-116">A: a titkosítással kapcsolatos házirendek eltávolítása nem eredményezi a konfigurált meghajtók visszafejtését.</span><span class="sxs-lookup"><span data-stu-id="80df0-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="80df0-117">K.: Miért jelzi, hogy az Intune megfelelőségi házirend azt mutatja, hogy az eszközön nincs "BitLocker enabled", de nem?</span><span class="sxs-lookup"><span data-stu-id="80df0-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="80df0-118">A: a "BitLocker enabled" beállítás az Intune megfelelőségi házirendjében a Windows-eszközök állapottanúsítvány-ügyfelét használja.</span><span class="sxs-lookup"><span data-stu-id="80df0-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="80df0-119">Ez az ügyfél csak a rendszerindítás során méri az eszköz állapotát.</span><span class="sxs-lookup"><span data-stu-id="80df0-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="80df0-120">Így ha egy eszköz nem lett újraindítva, mert a BitLocker-titkosítás befejeződött, a DHA Client szolgáltatás nem jelenti azt, hogy a BitLocker aktív marad.</span><span class="sxs-lookup"><span data-stu-id="80df0-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>