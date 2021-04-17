---
title: Bitlocker helyreállítási kulcsok
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820288"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="44890-102">A Bitlocker helyreállítási kulcsok elérése</span><span class="sxs-lookup"><span data-stu-id="44890-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="44890-103">A Bitlocker-beállítások Intune Endpoint Protection policy konfigurálásakor meg lehet határozni, hogy a Bitlocker helyreállítási információkat az Azure Active Directory tárolja-e.</span><span class="sxs-lookup"><span data-stu-id="44890-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="44890-104">Ha ez a beállítás be van állítva, akkor a tárolt helyreállítási adatoknak az Intune-rendszergazdáknak az Intune Devices blade eszközben tárolt eszközrekord-adatok részeként két módon kell láthatónak lenniük:</span><span class="sxs-lookup"><span data-stu-id="44890-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="44890-105">Eszközök – Azure AD-eszközök –> "Eszköz" VAGY Eszközök -> Minden eszköz -> "Eszköz" -> helyreállítási kulcsok</span><span class="sxs-lookup"><span data-stu-id="44890-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="44890-106">Ha maga az eszköz rendszergazdai hozzáféréssel rendelkezik, a helyreállítási kulcsot (Jelszó) a következő parancs rendszergazdai jogú parancssorból való futtatásával láthatja:</span><span class="sxs-lookup"><span data-stu-id="44890-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="44890-107">Ha az eszközt az Intune-ban való regisztráció előtt titkosították, előfordulhat, hogy a helyreállítási kulcsot az OOBE-folyamat során az eszközbe való bejelentkezéshez használt "Microsoft-fiók" (MSA) társította.</span><span class="sxs-lookup"><span data-stu-id="44890-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="44890-108">Ebben az esetben az MSA elérésének és az azzal való bejelentkezésnek meg kell mutatnia az eszközöket, amelyek helyreállítási kulcsait  https://onedrive.live.com/recoverykey tárolta.</span><span class="sxs-lookup"><span data-stu-id="44890-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="44890-109">Ha az eszközt tartományalapú csoportházirenden keresztül konfigurálva titkosította, a helyreállítási információkat a rendszer a számítógép active directoryjában tárolhatja.</span><span class="sxs-lookup"><span data-stu-id="44890-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="44890-110">Ha konfigurálta az Végpontvédelmi házirendet a helyreállítási kulcs Azure Active Directoryban való tárolására, de egy adott eszköz kulcsát még nem töltötte fel, a feltöltést úgy elindíthatja, hogy a mem konzolról elforgatja az adott eszköz helyreállítási kulcsát.</span><span class="sxs-lookup"><span data-stu-id="44890-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="44890-111">A részletekért [lásd: BitLocker helyreállítási kulcsok elforgatása.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="44890-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

