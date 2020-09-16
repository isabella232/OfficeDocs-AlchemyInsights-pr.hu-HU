---
title: Teams Felügyeleti központ
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670366"
---
# <a name="teams-admin-center"></a><span data-ttu-id="89464-102">Teams Felügyeleti központ</span><span class="sxs-lookup"><span data-stu-id="89464-102">Teams Admin Center</span></span>

<span data-ttu-id="89464-103">Megtudhatja, hogyan kezelheti a Teams alkalmazást a [Teams Felügyeleti központtal](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="89464-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="89464-104">Ha nem tudja elérni a Teams Felügyeleti központot, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="89464-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="89464-105">Győződjön meg arról, hogy engedélyezte a megfelelő [IP-címeket és URL-címeket az Office 365-höz](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) a peremhálózati eszközökön (tűzfalon stb.), illetve a helyi számítógépen beállított tűzfalszabályokban.</span><span class="sxs-lookup"><span data-stu-id="89464-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="89464-106">Győződjön meg arról, hogy a Teams felügyeleti portál eléréséhez használt bejelentkezési név megegyezik a [Microsoft 365 felügyeleti portálon](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) megadott felhasználónevével.</span><span class="sxs-lookup"><span data-stu-id="89464-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="89464-107">Ha nem jelennek meg felhasználók a Teams Felügyeleti központban, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="89464-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="89464-108">Létrehozott felhasználókat, vagy kiosztott licenceket az elmúlt 24 órában?</span><span class="sxs-lookup"><span data-stu-id="89464-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="89464-109">Kérjük, várjon legalább 24 órát, mielőtt támogatási jegyet nyitna.</span><span class="sxs-lookup"><span data-stu-id="89464-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="89464-110">Ellenőrizze: megfelelő licenceket rendelt hozzá a felhasználókhoz?</span><span class="sxs-lookup"><span data-stu-id="89464-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="89464-111">Ha helyszíni Active Directory-címtárral rendelkezik, győződjön meg arról, hogy [az msRTCSIP-PrimaryUserAddress vagy a SIP-cím értéke a helyi Active Directory-címtárban a ProxyAddresses mezőben látható, és a formátum megegyezik](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) a SIP: felhasználó**felhasználónevével** a [Microsoft 365 felügyeleti központjában](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="89464-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="89464-112">Ha meg kívánja őrizni a Skype vállalati verzió kiszolgálójának telepítési példányát, és a helyszíni és online otthoni felhasználóknak is elérhetővé szeretné tenni a felhasználókat, tegye a következőket: a **hibrid beállítás beállítása a Teams és a Skype vállalati online** verzióhoz a Skype vállalati verzió kiszolgálójának Vezérlőpultján, és helyezze át a felhasználókat az interneten.</span><span class="sxs-lookup"><span data-stu-id="89464-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
