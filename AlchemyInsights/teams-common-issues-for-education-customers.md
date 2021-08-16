---
title: A Teams gyakori problémái az oktatási ügyfelek számára
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 9dc01109d0f036c567243a8833a845f074097e39de4e1cfc1ba38da61b8f97ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049238"
---
# <a name="teams-common-issues-for-education-customers"></a>A Teams gyakori problémái az oktatási ügyfelek számára

**Oktatási felhasználóknak:**

Ha segítségre van szüksége a Teams telepítésével kapcsolatban a távoktatás támogatásához, kérjük, látogasson el a [FastTrack központba](https://www.microsoft.com/fasttrack) és küldjön el egy kérést. A Teams oktatási verzió ügyfeleinek a következő gyakori problémák fordulnak elő:

- Megjelent a „**Ne maradjon le semmiről!**“ üzenet? Feltétlenül [engedélyezze a Microsoft Teamst az iskolájának](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Az oktatási csomag bérlőiben a Microsoft Teams nincs alapértelmezés szerint engedélyezve; először be kell kapcsolnia azt.

- **Most ismerkedik a Teamsszel?** Ezután a [Távoli tanítás és tanulás az Office 365 Oktatási verzióban](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) című cikket tanulmányozva megismerheti az iskola beállítására, az óravázlat-tervezésre, a virtuális értekezletekre és a diákokkal való tartalommegosztásra vonatkozó legújabb útmutatót.

- Miután bekapcsolta a szolgáltatást, a felhasználók használhatják a Teams alkalmazást az [asztali-](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) és [mobilkliens](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients)telepítésével, vagy a https://teams.microsoft.com böngészőjéből.

- **Teams-vendéghozzáférés engedélyezése:** Tekintse át a [Teams vendéghozzáférésének ellenőrzőlistáját](https://docs.microsoft.com/microsoftteams/guest-access-checklist), és győződjön meg arról, hogy minden lépést elvégzett.
    - [A Microsoft Teamsbeli vendéghozzáférés ismertetése](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Beállítás – A Microsoft Teamsbeli vendéghozzáférés ellenőrzőlistája](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Vendég csatlakozása egy csapathoz](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams-értekezletek és betárcsázás**: Segítségre van szüksége a hangkonferencia bekapcsolásához vagy beállításához a Microsoft Teamsben? A felhasználó nemrégiben lett létrehozva? Ha igen, akkor a beállítások érvénybe lépéséhez várnia kell 2-24 órát. Ha ellenőrizni szeretné, hogy a felhasználó rendelkezik-e a hangkonferenciára vonatkozó licenccel és alapértelmezettként beállított nem ingyenes számmal:
    1. Válassza az Aktív felhasználók elemet, majd jelölje ki a kérdéses felhasználót.
    2. A felügyeleti központ verziójától függően válassza a **Licencek és appok** lehetőséget, vagy kattintson a **Szerkesztés** elemre a **Terméklicencek** panelen.
    3. Ellenőrizze, hogy a felhasználó rendelkezik-e licenccel a Hangkonferencia, Microsoft Teams és a Skype Vállalati online verzió (2. csomag) esetén.
    4. A Felügyeleti központokban kattintson **Az összes megjelenítése**, majd a **Teams** lehetőségre.
    5. A Microsoft Teams Felügyeleti központban kattintson az **Elavult portálverzió** lehetőségre.
    6. A Skype Vállalati verzió felügyeleti központjában kattintson a **hangkonferencia**, majd a **felhasználók** elemre.
    7. Jelölje ki a kérdéses felhasználót, és ellenőrizze, hogy a felhasználó rendelkezik-e alapértelmezett nem ingyenes telefonszámmal.

    További információért olvassa el a [Microsoft Teams Hívástervek](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) című cikket, vagy hívja a Microsoft kereskedelmi számlázási csapatát a licencelésre vonatkozó kérdésekkel kapcsolatos segítségért.

    További források

    - [Értekezletek és konferenciák a Microsoft Teamsben](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Hangkonferencia](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Értekezletszabályzatok**: Az értekezletszabályzatok használhatók a szervezete felhasználói által ütemezett értekezletek résztvevőinek elérhető funkciók szabályozásához. Miután létrehozott egy szabályzatot, és elvégezte a módosításokat, felhasználókat rendelhet a szabályzathoz.

    - **Értekezletszabályzat módosítása vagy létrehozása**: Ha értekezletszabályzatot szeretne módosítani vagy létrehozni, keresse meg a **Microsoft Teams Felügyeleti központ > Értekezletek > Értekezletszabályzatok** beállítást. Válasszon egy szabályzatot a listából, vagy válassza a **Hozzáadás** lehetőséget. Ha új szabályzatot hoz létre, adja meg a nevét és a leírását. A név nem tartalmazhat speciális karaktereket, és nem lehet hosszabb 64 karakternél. Adja meg a kívánt beállításokat, majd kattintson a **Mentés** gombra. 
    
        Tegyük fel például, hogy van néhány felhasználója, és korlátozni szeretné az értekezlethez szükséges sávszélességet. Érdemes létrehoznia egy „Korlátozott sávszélesség” nevű új szabályzatot és letiltani a következő beállításokat:

        A **Hang és videó** csoportban:
        - Kapcsolja ki a **Felhőalapú rögzítés engedélyezése** beállítást.
        - Kapcsolja ki az **IP-videó engedélyezése** beállítást.

        A **Tartalommegosztás** csoportban:

        - Tiltsa le a képernyőmegosztási módot.
        - Kapcsolja ki a **Rajztábla engedélyezése** beállítást.
        - Kapcsolja ki a **Megosztott jegyzetek engedélyezése** beállítást.

        Ezután **rendelje hozzá a szabályzatot a felhasználókhoz**:

    1. A Microsoft Teams Felügyeleti központ bal oldali navigációs panelén keresse meg a **Felhasználók** lehetőséget, és kattintson a felhasználóra.
    2. A felhasználónévtől balra kattintva jelölje ki a felhasználót, és kattintson a **Beállítások szerkesztése** lehetőségre.
    3. Az **Értekezletszabályzat** csoportban jelölje ki a hozzárendelni kívánt szabályzatot, majd kattintson az **Alkalmaz** gombra.

    Ha egyidejűleg több felhasználóhoz szeretne egy szabályzatot hozzárendelni, olvassa el a [Teams-felhasználóbeállítások tömeges szerkesztése](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk) című cikket.

    Teheti a következőket is:
    1. A Microsoft Teams Felügyeleti központ bal oldali navigációs panelén keresse meg az **Értekezletek > Értekezletszabályzatok** részt.
    2. Jelölje ki a szabályzatot a szabályzat nevétől balra kattintva.
    3. Kattintson a **Felhasználók kezelése** gombra.
    4. A **Felhasználók kezelése** panelen a megjelenítendő vagy a felhasználónév alapján keresse meg a felhasználót, majd kattintson a **Hozzáadás** gombra. Ismételje meg ezt a lépést minden hozzáadandó felhasználó esetében.
    5. Miután befejezte a felhasználók hozzáadását, kattintson a **Mentés** gombra.

- **Hibaelhárítás hiányzó tárcsázó esetén:**
    - Győződjön meg arról, hogy a felhasználó rendelkezik hozzárendelt [Teams-licenccel](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Győződjön meg arról, hogy a felhasználó rendelkezik hozzárendelt [híváscsomaggal](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Engedélyezze a felhasználóknak a [Vállalati hangkommunikációt](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Teams-bejelentkezés hibaelhárítása:** Először győződjön meg arról, hogy a [Microsoft Teams szolgáltatás működik](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Ezután keressen általános hibakódokat, és nézze át a következő cikket: [Miért tapasztalok problémát a Microsoft Teamsbe való bejelentkezéskor?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Érdemes lehet elolvasni az [Identitásmodellek és hitelesítés a Microsoft Teamsben](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication) című cikket is.
