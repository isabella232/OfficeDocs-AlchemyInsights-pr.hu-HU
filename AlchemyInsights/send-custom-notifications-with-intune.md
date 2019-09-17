---
title: Egyéni értesítések küldése az Intune szolgáltatással
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992315"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="d8e1d-102">Egyéni értesítések küldése kezelt iOS-és Android-eszközök felhasználóinak</span><span class="sxs-lookup"><span data-stu-id="d8e1d-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="d8e1d-103">Az Intune szolgáltatáshoz tartozó egyéni értesítéseket a felhasználó eszközén lévő Company Portal alkalmazás dolgozza fel.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="d8e1d-104">Az alkalmazás ezután létrehozza a leküldéses értesítést az eszközön.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="d8e1d-105">Az alábbi eszközelőfeltételek az egyéni értesítések kézhezvételének támogatásához, az alkalmazásnak pedig leküldéses értesítés létrehozásához:</span><span class="sxs-lookup"><span data-stu-id="d8e1d-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="d8e1d-106">Az eszköznek telepítve kell lennie a vállalati portál alkalmazással.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="d8e1d-107">Az eszköznek engedélyeznie kell a Company Portal alkalmazás számára a leküldéses értesítések küldését.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="d8e1d-108">Amikor az alkalmazás telepítve van vagy frissítve van, kérni fogja a felhasználót, hogy engedélyezze az értesítéseket.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="d8e1d-109">Az Android-eszközökön telepítve kell lennie a Google lejátszási szolgáltatásainak.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="d8e1d-110">Az eszközt az Intune-be kell beiratkozott.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="d8e1d-111">További információt az üzenet elküldéséről a [szolgáltatás dokumentációjában](https://docs.microsoft.com/intune/custom-notifications)talál.</span><span class="sxs-lookup"><span data-stu-id="d8e1d-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
