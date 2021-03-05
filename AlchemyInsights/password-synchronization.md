---
title: Jelszó-szinkronizálás
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482036"
---
# <a name="password-synchronization"></a><span data-ttu-id="69f4c-102">Jelszó-szinkronizálás</span><span class="sxs-lookup"><span data-stu-id="69f4c-102">Password synchronization</span></span>

<span data-ttu-id="69f4c-103">**A jelszó kivonat-szinkronizálása egyáltalán nem működik**</span><span class="sxs-lookup"><span data-stu-id="69f4c-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="69f4c-104">Egyes gyakori problémák az ügyfeleknél akkor találkoznak, ha a jelszó kivonat-szinkronizálása nem működik:</span><span class="sxs-lookup"><span data-stu-id="69f4c-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="69f4c-105">Az Azure AD Connect által a helyszíni Active Directoryval való  kommunikációhoz  használt Active Directory-fiók nem kap replikált címtárbeli módosításokat és replikált címtár-módosításokat minden engedélyt, amelyek a jelszó-szinkronizáláshoz szükségesek – ezt úgy kell kijavítani, hogy megadja ezeket az engedélyeket az Active Directory-fióknak.</span><span class="sxs-lookup"><span data-stu-id="69f4c-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="69f4c-106">A jelszó-kivonat szinkronizálása le van tiltva,  miután egy rendszergazda módosította a Felhasználói Sign-In-módszert jelszó-szinkronizálásról egy másik beállításra,  például az Összevonás az **AD FS** szolgáltatással az Azure AD Connect varázslóban – ezt az Azure AD Connect varázsló jelszó-kivonat-szinkronizálási funkciójának újra engedélyezésével oldhatja meg.</span><span class="sxs-lookup"><span data-stu-id="69f4c-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="69f4c-107">Kapcsolódási probléma a helyszíni Active Directoryval.</span><span class="sxs-lookup"><span data-stu-id="69f4c-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="69f4c-108">Egyes tartományvezérlők például nem érhetők el az Azure [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) AD Connect által, vagy a tűzfal blokkolja a szükséges portokat. Ezt úgy kell megoldania, hogy az Azure AD Connect-kiszolgáló és a helyszíni Active Directory közötti kapcsolat megfelelően működik.</span><span class="sxs-lookup"><span data-stu-id="69f4c-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="69f4c-109">Az Azure AD Connect-kiszolgáló jelenleg előkészítési módban van, ezért a kiszolgáló nem fogja tudni megadni a jelszó-előjeleket. A probléma megoldásához kövesse az [Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Connect-szinkronizálással való jelszó-szinkronizálás hibaelhárítása című szakasz lépéseit . A rendszer nem szinkronizál jelszavakat.</span><span class="sxs-lookup"><span data-stu-id="69f4c-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="69f4c-110">**A jelszó kivonat-szinkronizálása nem működik egyes felhasználóknál**</span><span class="sxs-lookup"><span data-stu-id="69f4c-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="69f4c-111">Ha azt vette észre, hogy egy felhasználó jelszavas  kivonata nem szinkronizálódik, az Azure AD Connect hibaelhárítási feladatával kivizsgálhatja és megoldhatja a problémát.</span><span class="sxs-lookup"><span data-stu-id="69f4c-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="69f4c-112">Végezze el az alábbi műveleteket:</span><span class="sxs-lookup"><span data-stu-id="69f4c-112">Perform the following tasks:</span></span>

    <span data-ttu-id="69f4c-113">a.</span><span class="sxs-lookup"><span data-stu-id="69f4c-113">a.</span></span> [<span data-ttu-id="69f4c-114">A hibaelhárítási feladat futtatása a varázslóban</span><span class="sxs-lookup"><span data-stu-id="69f4c-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="69f4c-115">b.</span><span class="sxs-lookup"><span data-stu-id="69f4c-115">b.</span></span> [<span data-ttu-id="69f4c-116">A hibaelhárítási parancsmag használatával vizsgálja meg egy adott használat jelszó kivonatszinkronizálási problémáit.</span><span class="sxs-lookup"><span data-stu-id="69f4c-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="69f4c-117">A helyszíni Active Directory user objektum engedélyezve van a Felhasználó számára, és a következő **bejelentkezéskor módosítania** kell a jelszót.</span><span class="sxs-lookup"><span data-stu-id="69f4c-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="69f4c-118">Ha ez a beállítás engedélyezve van, a felhasználóhoz egy ideiglenes jelszó lesz rendelve, és a rendszer kérni fogja, hogy módosítsa a jelszót a következő bejelentkezéskor.</span><span class="sxs-lookup"><span data-stu-id="69f4c-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="69f4c-119">Az Azure AD Connect nem szinkronizálja az ideiglenes jelszavakat az Azure AD-be.</span><span class="sxs-lookup"><span data-stu-id="69f4c-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="69f4c-120">A fenti probléma megoldásához végezze el az alábbi műveletek egyikét:</span><span class="sxs-lookup"><span data-stu-id="69f4c-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="69f4c-121">Kérje meg a felhasználót, hogy jelentkezzen be a helyszíni alkalmazásba (például asztali Windowsba), és módosítsa a jelszót.</span><span class="sxs-lookup"><span data-stu-id="69f4c-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="69f4c-122">Az új jelszó szinkronizálva lesz az Azure AD-vel.</span><span class="sxs-lookup"><span data-stu-id="69f4c-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="69f4c-123">A következő bejelentkezéskor a felhasználónak módosítania kell a jelszót, és meg kell osztania a felhasználóval az új jelszót. </span><span class="sxs-lookup"><span data-stu-id="69f4c-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="69f4c-124">A helyszíni Active Directory-felhasználó  objektum nincs megfelelően konfigurálva az objektum-szinkronizáláshoz vagy a jelszó-szinkronizáláshoz.</span><span class="sxs-lookup"><span data-stu-id="69f4c-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="69f4c-125">A probléma megoldásához kövesse az Azure AD Connect szinkronizálásával való jelszó-kivonat-szinkronizálás hibaelhárítása [témakörben leírt lépéseket.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="69f4c-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







