---
title: Csoportproblémák elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714055"
---
# <a name="troubleshoot-group-issues"></a>Csoportproblémák elhárítása

**Azure AD-szerepkörhöz kell hozzárendelnem egy csoportot**

Ha Azure Active Directory -csoportot szeretne hozzárendelni egy Azure AD-szerepkörhöz, kövesse az alábbi lépéseket:

1. Új csoport létrehozása – Új csoport létrehozása:

    a. Jelentkezzen be az Azure AD Felügyeleti központba jogosultsággal rendelkező szerepkörgazdával vagy globális rendszergazdai engedélyekkel. 
    b. Válassza az Azure Active Directory > Csoportok > Új > csoportban. 
    c. Hozza létre a csoportot.

2. Rendelje hozzá a szerepkört a csoporthoz a csoport létrehozásakor vagy a csoport létrehozása után.

    a. Ha a csoport létrehozásakor szerepkört szeretne hozzárendelni a csoporthoz, kapcsolja be az Azure AD-szerepköröket a csoporthoz rendelve és hozza létre a csoportot.
    b. Ha a létrehozása után hozzá szeretne rendelni egy szerepkört a csoporthoz, nyissa meg az újonnan létrehozott csoport Hozzárendelt szerepkörök lapját, és rendelje hozzá a szerepkört a csoporthoz.

**Azure AD-szerepkörhöz hozzárendelt csoport tagságát kell kezelnem**

1. A jogosultságok kiterjesztésének megakadályozása érdekében alapértelmezés szerint csak a jogosultsággal rendelkező szerepkör rendszergazdája és a globális rendszergazda módosíthatja egy szerepkörhöz hozzárendelt csoport tagságát. Dönthetnek azonban úgy, hogy tulajdonost rendelnek egy ilyen csoporthoz, és delegálják ezt a feladatot. További információért lásd: Szerepkör-hozzárendelések kezelése felhőalapú csoportokkal az [Azure Active Directoryban.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Az Azure AD-beli csoportokhoz való szerepkörök hozzárendelésére vonatkozó gyakori kérdéseket és hibaelhárítási tippeket a felhőbeli csoportokhoz rendelt szerepkörök [hibaelhárítása témakörben talál.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Dinamikus csoportok**

1. Ha nem találja a beépített felhasználói attribútumokat, győződjön meg arról, hogy az attribútum szerepel a támogatott tulajdonságok listájában.
2. Ha beépített eszközattribútumokat keres, győződjön meg arról, hogy az attribútum szerepel az eszközattribútumok listájában. 
3. A beépített felhasználói és eszközattribútumok mellett bővítményattribútumokat is [használhat.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Miután szinkronizálta a bővítményattribútumokat a helyszíni Windows Server AD-ről vagy egy csatlakoztatott SaaS-alkalmazásból, az attribútumok láthatónak kell lenniük a szabályszerkesztő legördülő listájában. Az egyéni attribútum neve megtalálható a címtárban úgy, hogy lekérdezi egy felhasználó attribútumát a PowerShell használatával, és rákeres az attribútum nevére. Ezek a szabályok a szabályok szintaxisában is használhatók.
4. Győződjön meg arról, hogy a bérlő rendelkezik a megfelelő licenccel. A dinamikus csoportokhoz a bérlőnek Azure AD P1 Premium licenccel kell rendelkezik. Az Azure AD licenctervek listája itt [érhető el.](https://azure.microsoft.com/pricing/details/active-directory/) A Nagyvállalati mobilitási és biztonsági licencelési csomagok itt [érhetők el.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Győződjön meg arról, hogy a dinamikus csoportot létrehozására használó felhasználó szerepköre globális rendszergazda, Intune-rendszergazda, csoport- vagy felhasználó-rendszergazda.
6. Kérjük, hagyja, hogy a csoport kitöltsen egy időt. A bérlői webhely méretétől függően akár 24 óra is eltelhet, amikor a csoport első alkalommal vagy szabályváltozás után újra megjelenik.
7. További információ: [Attribútumalapú szabályok létrehozása a dinamikus csoporttagsághoz.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Törölnem kell egy csoportot**

1. A csoportok törölhetők a címtárból az Azure AD Powershell Remove-AzureADGroup parancsmag használatával.
2. Mielőtt megpróbál törölni egy szinkronizált csoportot az Azure AD-ben, a hibák elkerülése érdekében győződjön meg arról, hogy törölte az összes hozzárendelt licencet.
3. A csoportok törléséről további információt a Hozzárendelt licenccel rendelkező csoportok [törlése.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Törölt csoportot kell visszaállítanom**

1. Ha töröl egy Office 365-csoportot, az csak 30 nappal a végleges törlés előtt állítható vissza. A végleges törlés után a csoport többé nem állítható vissza. A csoportok visszaállításáról itt [olvashat bővebben.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Ez a funkció biztonsági csoportok és terjesztési csoportok esetén nem támogatott.
3. Győződjön meg arról, hogy jogosult egy Office 365-csoport visszaállítására. A globális rendszergazdák, a csoport-rendszergazdák, a felhasználói fiókok rendszergazdái, az Intune szolgáltatás-rendszergazdái, a partnerszint1- vagy a tier2-támogatás, valamint a csoport tulajdonosa visszaállíthat egy csoportot.
4. Amikor egy dinamikus csoportot törölnek és visszaállítnak, azt egy új csoportnak juk, majd a szabálynak megfelelően újra feltöltjük. Ez a folyamat akár 24 órát is igénybe vehet.
5. A törölt csoportok visszaállításáról további információt [a Törölt Office 365-csoportok](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)visszaállítása az Azure Active Directoryban.

**Csoport lejárati házirend-konfigurációja**

1. Ez a funkció csak Office 365-csoportok esetén támogatott, biztonsági csoportok és terjesztési csoportok esetében nem.
2. Az Office 365-csoportok lejárati házirendének konfigurálásához és használatához Azure AD Premium-licenc szükséges.
3. Jelenleg csak egy lejárati házirend konfigurálható az Office 365-csoportokhoz a bérlői webhelyen.
4. Csak globális rendszergazdák, csoport-rendszergazdák, felhasználó-rendszergazdák és a csoport tulajdonosa újíthat meg csoportokat.
5. Ha egy Office 365-csoport lejárt, az törlődik, és csak 30 nappal a végleges törlés előtt állítható vissza. A végleges törlés után a csoport többé nem állítható vissza. A csoportok visszaállításáról itt [olvashat bővebben.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Tevékenységalapú automatikus megújítás**

A SharePointból, az Outlookból és a Teamsből származó felhasználói tevékenységek kiválthatja a csoportok automatikus megújítását. A tevékenységeket a csoport lejárata előtt 35 nappal ellenőrzi a program. Ha a csoport aktuális életciklusa alatt tevékenység történik, a csoport automatikusan megújul, és nem küld e-mailes értesítést a csoporttulajdonosoknak.

**Lejárt csoportok értesítési időzítése**

1. Az e-mail-értesítéseket a rendszer a csoport lejárata előtt 30, 15 nappal és 1 nappal azelőtt küldi el az Office 365-csoporttulajdonosoknak, hogy elévülnek.
2. A lejárat első beállításakor a lejárati intervallumnál régebbi csoportok a lejáratig 35 napra vannak állítva.
3. A csoport lejárati dátumát nem a házirend frissítésének dátuma, de a rendszer a csoport megújítási dátuma alapján számítja ki. Ha a lejárati házirend frissül, a lejárati dátum nem változik.
4. További információt a [](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) Csoport lejárati házirendje és az e-mailek megújítása, valamint egy törölt [Office 365-csoport](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)visszaállítása az Azure Active Directoryban.

**Csoport létrehozására vonatkozó engedély**

Győződjön meg arról, hogy jogosult új csoport létrehozására. A globális rendszergazdák letilthatják a csoportok létrehozását az Azure Portalon vagy az Access panelen. Szükség lehet egy rendszergazdára az új csoport létrehozásához vagy a megfelelő engedélyek létrehozására.

1. [Új csoport létrehozása és tagok hozzáadása az Azure Portalon](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Csoportok létrehozása a PowerShell MSOnline-ban](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Csoportok létrehozásának letiltása a PowerShellben](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Csoportok létrehozására képes felhasználók kezelése az Office 365-ben](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Az Office 365 üdvözlő értesítésének letiltása a Powershellen keresztül](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD rendszergazdai szerepkörök](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Csoport létrehozási engedélyeinek kezelése**

1. A globális rendszergazdák kezelhetik az Azure Portálon vagy az Access panelen létrehozott biztonsági csoportok vagy Office 365-csoportok csoport létrehozási engedélyét úgy, hogy a Felhasználók biztonsági csoportokat hozhatnak létre az **Azure-portálon,** illetve a felhasználók Office **365-csoportokat** hozhatnak létre az Azure Portals minden > **Általános (Beállítások)** csoportjában.
2. Ha Azure AD P1 Prémium verziós licenccel rendelkezik, korlátozhatja a csoportok létrehozását, és így kijelölheti a felhasználók egy csoportját.

**Az Office 365-csoport új tagjainak üdvözlő értesítésének letiltása**

Az Office 365-csoportokba felvett felhasználóknak küldött üdvözlő értesítés letiltható a Hamis érték `UnifiedGroupWelcomeMessageEnabled` powershellben való  beállításával. Erről a beállításról itt [olvashat.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













