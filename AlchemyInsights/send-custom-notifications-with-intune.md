---
title: Egyéni értesítések küldése a Intune szolgáltatással
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720648"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="056a2-102">Egyéni értesítések küldése a felügyelt iOS-és Android-eszközök felhasználóinak</span><span class="sxs-lookup"><span data-stu-id="056a2-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="056a2-103">Az Intune-alapú egyéni értesítéseket a vállalati portál alkalmazás dolgozza fel a felhasználó eszközén.</span><span class="sxs-lookup"><span data-stu-id="056a2-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="056a2-104">Az App ekkor létrehozza a leküldéses értesítést az adott eszközön.</span><span class="sxs-lookup"><span data-stu-id="056a2-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="056a2-105">Az alábbi eszközök előfeltételei az egyéni értesítések beérkezésének támogatása, és az alkalmazás ekkor hozza létre a leküldéses értesítést:</span><span class="sxs-lookup"><span data-stu-id="056a2-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="056a2-106">Az eszköznek telepítve kell lennie a vállalati portál alkalmazásnak.</span><span class="sxs-lookup"><span data-stu-id="056a2-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="056a2-107">Az eszköznek engedélyeznie kell a vállalati portál alkalmazás leküldéses értesítések küldését.</span><span class="sxs-lookup"><span data-stu-id="056a2-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="056a2-108">Az alkalmazás telepítésekor vagy frissítésekor a rendszer rákérdez a felhasználótól, hogy engedélyezze az értesítéseket.</span><span class="sxs-lookup"><span data-stu-id="056a2-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="056a2-109">Android-eszközökön telepítve kell lennie a Google Play Services szolgáltatásnak.</span><span class="sxs-lookup"><span data-stu-id="056a2-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="056a2-110">Az eszközt a Intune szolgáltatással kell regisztrálni.</span><span class="sxs-lookup"><span data-stu-id="056a2-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="056a2-111">Az üzenetek küldéséről további információt a [funkció dokumentációjában](https://docs.microsoft.com/intune/custom-notifications)talál.</span><span class="sxs-lookup"><span data-stu-id="056a2-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
