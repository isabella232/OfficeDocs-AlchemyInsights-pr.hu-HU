---
title: BitLocker helyreállítási kulcsok
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685888"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="7a945-102">Hozzáférés a BitLocker helyreállítási kulcsaihoz</span><span class="sxs-lookup"><span data-stu-id="7a945-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="7a945-103">A BitLocker-beállítások Intune-végpontok védelmi házirendjének konfigurálásakor meghatározhatja, hogy a BitLocker helyreállítási információkat az Azure Active Directoryban kell-e tárolni.</span><span class="sxs-lookup"><span data-stu-id="7a945-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="7a945-104">Ha ez a beállítás be van állítva, akkor a tárolt helyreállítási adatoknak a Intune-rendszergazdák számára kétféleképpen kell szerepelniük az Intune-eszközök lapon, a következő két módon:</span><span class="sxs-lookup"><span data-stu-id="7a945-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="7a945-105">Eszközök – Azure AD-eszközök – > "eszköz" vagy eszközök – > minden eszköz – > "eszköz" – > helyreállítási kulcsok</span><span class="sxs-lookup"><span data-stu-id="7a945-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="7a945-106">Azt is megteheti, hogy az eszközhöz rendszergazdai hozzáférés van megnyitva, a helyreállítási kulcs (jelszó) a következő parancs futtatásával tekinthető meg egy rendszergazdai jogú parancssorból:</span><span class="sxs-lookup"><span data-stu-id="7a945-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="7a945-107">Ha az eszköz az Intune-ba való bejelentkezés előtt titkosított, lehet, hogy a helyreállítási kulcs társítva van a Microsoft-fiókhoz (MSA), amellyel az OOBE folyamat során bejelentkezhet az eszközre.</span><span class="sxs-lookup"><span data-stu-id="7a945-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="7a945-108">Ebben az esetben a MSA való hozzáférés  https://onedrive.live.com/recoverykey és bejelentkezés során meg kell jeleníteni azokat az eszközöket, amelyekhez a helyreállítási kulcsokat tárolták.</span><span class="sxs-lookup"><span data-stu-id="7a945-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="7a945-109">Ha az eszköz tartományon alapuló csoportházirend-konfiguráción keresztül volt titkosítva, a helyreállítási adatok a helyszíni Active Directoryban tárolhatók.</span><span class="sxs-lookup"><span data-stu-id="7a945-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

