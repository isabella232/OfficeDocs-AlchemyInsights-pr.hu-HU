---
title: Egyéni értesítések küldése az Intune szolgáltatással
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886859"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="3874a-102">Egyéni értesítések küldése kezelt iOS-és Android-eszközök felhasználóinak</span><span class="sxs-lookup"><span data-stu-id="3874a-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="3874a-103">Az Intune szolgáltatáshoz tartozó egyéni értesítéseket a felhasználó eszközén lévő Company Portal alkalmazás dolgozza fel.</span><span class="sxs-lookup"><span data-stu-id="3874a-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="3874a-104">Az alkalmazás ezután létrehozza a leküldéses értesítést az eszközön.</span><span class="sxs-lookup"><span data-stu-id="3874a-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="3874a-105">Az alábbi eszközelőfeltételek az egyéni értesítések kézhezvételének támogatásához, az alkalmazásnak pedig leküldéses értesítés létrehozásához:</span><span class="sxs-lookup"><span data-stu-id="3874a-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="3874a-106">Az eszköznek telepítve kell lennie a vállalati portál alkalmazással.</span><span class="sxs-lookup"><span data-stu-id="3874a-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="3874a-107">Az eszköznek engedélyeznie kell a Company Portal alkalmazás számára a leküldéses értesítések küldését.</span><span class="sxs-lookup"><span data-stu-id="3874a-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="3874a-108">Amikor az alkalmazás telepítve van vagy frissítve van, kérni fogja a felhasználót, hogy engedélyezze az értesítéseket.</span><span class="sxs-lookup"><span data-stu-id="3874a-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="3874a-109">Az Android-eszközökön telepítve kell lennie a Google lejátszási szolgáltatásainak.</span><span class="sxs-lookup"><span data-stu-id="3874a-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="3874a-110">Az eszközt az Intune-be kell beiratkozott.</span><span class="sxs-lookup"><span data-stu-id="3874a-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="3874a-111">További információt az üzenet elküldéséről a [szolgáltatás dokumentációjában](https://docs.microsoft.com/intune/custom-notifications)talál.</span><span class="sxs-lookup"><span data-stu-id="3874a-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
