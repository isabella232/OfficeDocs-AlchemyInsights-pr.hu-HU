---
title: Eszközpin/jelszó alaphelyzetbe állítása az Intune-ból
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: fd3bb957b0da22dfab5a9988a82e398757e12ee5
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439431"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="121ca-102">Eszközpin/jelszó alaphelyzetbe állítása az Intune-ból</span><span class="sxs-lookup"><span data-stu-id="121ca-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="121ca-103">A jelkód eltávolítása vagy a Jelszó eltávolítása művelettel kényszerítheti a felhasználót, hogy hozzon létre egy új jelszót az Intune-ban egy iOS vagy Android rendszert futtató eszközhöz.</span><span class="sxs-lookup"><span data-stu-id="121ca-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="121ca-104">Ezt a műveletet csak bizonyos operációsrendszer-típusok és munkaprofil-típusok támogatják.</span><span class="sxs-lookup"><span data-stu-id="121ca-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="121ca-105">A támogatott platformokról és az alaphelyzetbe állítási jelkód művelet elindításáról az [Eszköz jelkódjának visszaállítása vagy eltávolítása az Intune-ban című témakörben talál.](https://docs.microsoft.com/intune/device-passcode-reset)</span><span class="sxs-lookup"><span data-stu-id="121ca-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="121ca-106">A Windows 10 Mobile operációs rendszert futtató eszközökön a Pin Reset művelettel visszaállíthatja a meglévő pineket egy új értékre.</span><span class="sxs-lookup"><span data-stu-id="121ca-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="121ca-107">Ez lehetővé teszi a felhasználó számára, hogy feloldja az eszközt, és szükség szerint új pint állítson be.</span><span class="sxs-lookup"><span data-stu-id="121ca-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="121ca-108">További információt [a Jelkód visszaállítása Windows-eszközökön az Intune használatával című](https://docs.microsoft.com/intune/device-windows-pin-reset)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="121ca-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>