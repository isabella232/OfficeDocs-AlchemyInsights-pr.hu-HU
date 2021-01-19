---
title: Felhasználói problémák elhárítása
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901039"
---
# <a name="announcements"></a>Hirdetmények

A Google kompatibilitás tesztelésére vonatkozó útmutatását követve tesztelje, hogy az ön alkalmazásai érintettek-e. A Google útmutatója elérhető a https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Ha felhasználóit fogyasztói Google-fiókkal jelentkezik be, győződjön meg arról, hogy a rendszer webmegtekintőjét vagy a rendszerböngészőt használja. További információt a Csak a Chrome böngészővel való [alkalmazás(ak)ba](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)való bejelentkezés során problémákat tartalmaz.


**Nem tudok új felhasználót létrehozni az Azure AD címtárban**

Az alábbi lépésekkel elháríthatja azt a problémát, amely miatt nem lehet új felhasználót létrehozni az Azure AD-ban:

1. Győződjön meg arról, hogy jogosult új normál felhasználó létrehozására. Új normál felhasználót csak az Azure Active Directory (AD) globális rendszergazdája vagy felhasználó-rendszergazdai szerepköre hozhat létre. Ha nem ilyen szerepkörben van, kérje meg a rendszergazdát, hogy vegye fel az egyik ilyen szerepkörbe, vagy hozza létre az új felhasználói fiókot.
2. Győződjön meg arról, hogy a felhasználónév az Azure AD-ban ellenőrzött tartományban található. Ha nem található igazolt egyéni tartománynév az Azure AD-ban, használhatja az Azure AD kezdeti tartományát, amelynek végén *.onmicrosoft.com.
3. Győződjön meg arról, hogy a felhasználónév olyan tartományban van, amely nincs az Azure AD-hez egyesítve a helyszíni AD-től. A felhőbe nem lehet felhasználókat hozzáadni helyszíni összevont tartománynevekkel.
4. Győződjön meg arról, hogy egy másik felhasználó vagy partner sem rendelkezik az új felhasználóhoz hozzárendelni kívánt felhasználónévvel. A felhasználóneveknek egyedinek kell lennie az Azure AD-ban.
5. Az [Azure AD szerepköreit](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) és rendszergazdáit az Azure AD szolgáltatásban láthatja.
6. Tekintse meg [az](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) Azure AD tartománynevét.
7. A [naplókat áttekintve](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) részletesebb információkat láthat egy nemrég létrehozott vagy törölt felhasználóról, például arról, hogy ki és mikor hajtotta végre a műveletet.
8. Az új felhasználók hozzáadásáról további információt az Azure AD-beli új felhasználók létrehozása az [Azure Portal használatával.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
9. Az Azure AD rendszergazdai szerepköreinek engedélyeit az Azure AD rendszergazdai [szerepköreinek használatával kapcsolatos további információkért lásd: Azure AD-rendszergazdai szerepkörök.](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
10. A felhasználók Azure AD Powershell használatával való létrehozásáról az [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)segítségével hozhat létre új felhasználót.

**Probléma az önkiszolgáló regisztrációval**

Az önkiszolgáló regisztrációval kapcsolatos hibák elhárításához végezze el az alábbi lépéseket:

1. Ha önkiszolgáló regisztrációt használ az alkalmazásokkal, először engedélyezze az önkiszolgáló regisztrációt a bérlői webhelyen. 
2. Ha engedélyezni szeretné egy alkalmazásnak az önkiszolgáló regisztrációt, vegye fel a felhasználói folyamatba. Amikor legközelebb az alkalmazás bejelentkezési lapjára keres fel egy lehetőséget,*_*Nincs fiók? Hozzon létre egyet!_* _. Ezzel elindítja az önkiszolgáló regisztrációt.
3. Az Önkiszolgáló regisztráció használatával az Azure AD szolgáltatásban a szervezet feltöltésére vonatkozó információkért lásd: Önkiszolgáló regisztráció az [Azure AD szolgáltatásra.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)
4. Miután társítja a felhasználói folyamatot egy vagy több alkalmazással, az adott appot felkereső felhasználók a felhasználói folyamat beállításaival regisztrálnak és vendégfiókot szereznek be. A vendégfiókok regisztrációjára és elnyerésére vonatkozó további információkért a felhasználók láthatják a vendégfelhasználók önkiszolgáló [regisztrációját.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)

_ *Probléma külső felhasználó meghívása**

A külső felhasználók meghívásával kapcsolatos hibák elhárításához végezze el az alábbi lépéseket:

Győződjön meg arról, hogy a felhasználó meghívóját arra az e-mail-címre küldte el, amely megegyezik azzal a névvel, amelybe a felhasználó bejelentkezik. Ha elküldi a meghívót egy felhasználó proxy e-mail-címére, a felhasználó nem tudja beváltani. További információt az [Azure AD B2B dokumentációjában talál.](https://docs.microsoft.com/azure/active-directory/external-identities/)

**Nem tudok licenceket hozzárendelni egy felhasználóhoz**

A licencek felhasználóhoz való hozzárendelésével kapcsolatos hibák elhárításához végezze el az alábbi lépéseket:

1. A felhasználói licencek kezeléséhez győződjön meg arról, hogy olyan fiókot használ, amely a szükséges rendszergazdai szerepkörök valamelyikével rendelkezik: globális rendszergazda, licenc-rendszergazda vagy felhasználó-rendszergazda. A felhasználó szerepkörét a felhasználói  panel Címtár szerepkör lapján ellenőrizheti.
2. Ha az Azure Portalot használja, és a licenc-hozzárendelés sikertelen, kattintson a jobb felső sarokban lévő értesítésre. Ezzel megnyit egy panelt, amely részleteket tartalmaz arról, hogy mi történt. A legtöbb esetben ez elegendő a probléma megértő és megoldható megoldásához.
3. Mielőtt hozzárendelhet egy licencet egy felhasználóhoz, győződjön meg arról, hogy a **Használati hely** tulajdonság be van állítva a felhasználóhoz. Ellenőrizze, hogy a felhasználó beállította-e a tulajdonságot a felhasználói panel **Profil** lapján.
4. Győződjön meg arról, hogy elegendő licenc áll rendelkezésre a hozzárendelni próbált termékhez. A rendelkezésre álló licencek számát az Azure Portal webhelyen, az [Azure Active Directory -> -> Minden termék webhelyen láthatja.](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)
5. Előfordulhat, hogy a felhasználónak már van egy másik licence, amelynek a szolgáltatásai ütköznek a hozzárendelni próbált új licencben megadott szolgáltatásokkal. Ha például a felhasználónál engedélyezve van az Exchange Online (1. csomag) szolgáltatás, akkor nem tud licencet hozzárendelni az Exchange Online-hoz (2. csomag). Az új licenc-hozzárendelés engedélyezése érdekében tiltsa le az egyik szolgáltatást. Az Azure Portal vagy a PowerShell-parancsmagok  használata esetén a probléma részleteit tartalmazó lapon megjelennek az ütközést okozó szolgáltatások.
6. Ha megpróbál eltávolítani egy licencet, de ez nem sikerül, előfordulhat, hogy a felhasználónak más licencei is vannak az eltávolítani próbált szolgáltatásoktól függő szolgáltatásokkal. Az Azure Portal vagy a PowerShell-parancsmagok használata esetén a hibaüzenet felsorolja a függőségekkel kapcsolatos szolgáltatásokat.
7. Ha szeretné megérteni, hogy miért adtak hozzá/távolított el egy licencet egy felhasználótól (például hogy ki más végzett még módosításokat a szervezetben), ellenőrizze a naplókat. Állítsa a szűrőt **licenctevékenységre** úgy, hogy az az összes módosítást mutassa, beleértve az azokat végrehajtott "szereplőt" is.
8. Ha Exchange Online-t használ, előfordulhat, hogy a bérlő néhány felhasználója helytelenül van beállítva ugyanazokkal a proxycímekkel. Ilyen esetekben általános hibaüzenetek jelenhetnek meg, ha egy licencművelet meghiúsul. [Ez a cikk](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) további információkat tartalmaz a problémáról, többek között arról, hogy miként csatlakozhat az [Exchange Online-hoz távoli PowerShell használatával.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) Ha meg kell határoznia, hogy a bérlői webhely mely felhasználói ugyanazt a proxycímet tartalmazzák, hajtsa végre ezt az Exchange Online-parancsmagot:

Futtatás

Get-Recipient | ahol {$_. EmailAddresses -match <user principal name> } | fL Name, RecipientType,emailaddresses





