---
title: A 0x8004de40 kijavítva a OneDrive-ban
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649750"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b92b5-102">A 0x8004de40 kijavítva a OneDrive-ban</span><span class="sxs-lookup"><span data-stu-id="b92b5-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b92b5-103">Ha Windows 7 rendszert használ, és ez a hibaüzenet jelenik meg, a Frissítés az alapértelmezett biztonságos protokollként való [TLS 1.1 és TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)engedélyezéséhez a Windows rendszerbenHTTP.</span><span class="sxs-lookup"><span data-stu-id="b92b5-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="b92b5-104">Ha Windows 10 rendszert futtat, és egy hibaüzenet 0x8004de40 OneDrive-val:</span><span class="sxs-lookup"><span data-stu-id="b92b5-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b92b5-105">Indítsa újra az érintett számítógépet, miközben az Acitve-címtár tartományához csatlakozik.</span><span class="sxs-lookup"><span data-stu-id="b92b5-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b92b5-106">Ha egy újraindítás nem oldja meg a problémát, oldja fel az eszközhöz való, majd az Azure AD-ból való újracsatlakozáskor.</span><span class="sxs-lookup"><span data-stu-id="b92b5-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b92b5-107">**Megjegyzés:** A lépések végrehajtása közben a vállalati hálózatnak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="b92b5-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b92b5-108">Ne hajtsa végre ezeket a lépéseket, ha nem csatlakozik vállalati infrastruktúrához (például utazás közben).</span><span class="sxs-lookup"><span data-stu-id="b92b5-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="b92b5-109">Nyisson meg egy rendszergazdai jogú parancssort a **Start** menüből, kattintson a jobb gombbal a **Parancssor** elemre, majd válassza a **Futtatás rendszergazdaként parancsot.**</span><span class="sxs-lookup"><span data-stu-id="b92b5-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="b92b5-110">Írja *be a dsregcmd /leave parancsot, és* nyomja le az Enter **billentyűt.**</span><span class="sxs-lookup"><span data-stu-id="b92b5-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="b92b5-111">Ha elkészült, írja be a *dsregcmd /join parancsot,* és nyomja le az **Enter billentyűt.**</span><span class="sxs-lookup"><span data-stu-id="b92b5-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="b92b5-112">Ha elkészült, zárja be a parancssort.</span><span class="sxs-lookup"><span data-stu-id="b92b5-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="b92b5-113">Indítsa újra a számítógépet, és jelentkezzen be a OneDrive-ba.</span><span class="sxs-lookup"><span data-stu-id="b92b5-113">Reboot the computer, and log into OneDrive.</span></span>