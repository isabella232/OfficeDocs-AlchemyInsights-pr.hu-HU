---
title: Jelszóvisszaírás engedélyezése Azure AD Connect szolgáltatásban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093357"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e6b4f-102">Jelszóvisszaírás engedélyezése Azure AD Connect szolgáltatásban</span><span class="sxs-lookup"><span data-stu-id="e6b4f-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e6b4f-103">Az önkiszolgáló jelszó-visszaállítás visszaírásának engedélyezéséhez először engedélyezze a visszaírást az Azure AD Connect szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e6b4f-104">Az Azure Active Directory Connect kiszolgálóról hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="e6b4f-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e6b4f-105">Lépjen be Azure AD Connect kiszolgálóra, és indítsa el az **Azure AD Connect** konfiguráló varázslót.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e6b4f-106">Az **Üdvözlőlapon** kattintson a **Konfigurálás** gombra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e6b4f-107">A **További tevékenységek** oldalon jelölje be a **Szinkronizálási beállítások testre szabása** elemet, majd kattintson a **Következő** gombra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e6b4f-108">A **Csatlakozás az Azure Active Directory szolgáltatáshoz** oldalon adjon meg egy globális rendszergazda hitelesítő adatot az Azure bérlőjéhez, majd kattintson a **Következő** gombra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e6b4f-109">A **Címtárak csatlakoztatása** és **Tartomány/szervezeti egységek** szűrése lapokon kattintson a **Következő** gombra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e6b4f-110">A **Választható funkciók** oldalon jelölje be a **Jelszóvisszaírás** melletti jelölőnégyzetet, majd kattintson a **Következő** gombra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e6b4f-111">A **Konfigurálásra kész** oldalon kattintson a **Konfigurálás** gombra, majd várja meg, hogy a folyamat befejeződjön.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e6b4f-112">Ha úgy látja, hogy befejeződött a folyamat, kattintson a **Kilépés** gombra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e6b4f-113">Ha engedélyezve van a jelszóvisszaírás az Azure AD Connect eszközön, állítsa be az Azure AD SSPRT-t visszaírásra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e6b4f-114">A visszaírás SSPR-ben való engedélyezéséhez hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="e6b4f-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e6b4f-115">Jelentkezzen be az Azure Portal webhelyre egy globális rendszergazdai fiókkal.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e6b4f-116">Keresse meg és jelölje be az **Azure Active Directory** elemet, kattintson a **Jelszó alaphelyzetbe állítása**, majd a **Helyszíni integráció** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e6b4f-117">Állítsa a **Jelszavak visszaírása a helyszíni címtárakba?** beállítást **Igen** értékre.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e6b4f-118">Állítsa a **Felhasználói fiókok visszaállításának engedélyezése a jelszó alaphelyzetbe állítása nélkül?** beállítást **Igen** értékre.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e6b4f-119">Ha elkészült, kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e6b4f-120">További információért lásd: [Azure Active Directory önkiszolgáló jelszó-visszaállítási visszaírás engedélyezése egy helyszíni környezethez](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="e6b4f-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e6b4f-121">Amikor egy rendszergazda alaphelyzetbe állítja egy felhasználó jelszavát az Azure Portal webhelyen, ha az adott felhasználó összevont felhasználó vagy a jelszókivonatok szinkronizálva vannak, a rendszer a jelszót visszaírja a helyszíni környezetbe.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e6b4f-122">Ehhez a funkcióhoz Azure Premium-licenc (P1 vagy P2) szükséges, és jelenleg nem támogatott az Office Felügyeleti portálon.</span><span class="sxs-lookup"><span data-stu-id="e6b4f-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
