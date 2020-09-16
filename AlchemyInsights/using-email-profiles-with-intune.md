---
title: E-mail-profilok használata a Intune szolgáltatással
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653290"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="0dcf2-102">E-mail-profilok használata a Intune szolgáltatással</span><span class="sxs-lookup"><span data-stu-id="0dcf2-102">Using email profiles with Intune</span></span>

<span data-ttu-id="0dcf2-103">Az Intune segítségével a natív (beépített) levelezőprogram e-mail-profiljait több eszköz platformon is létrehozhatja és telepítheti.</span><span class="sxs-lookup"><span data-stu-id="0dcf2-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="0dcf2-104">A levelezési profilokkal kapcsolatos néhány korlátozásról, például a meglévő profilok kezelési módjáról és a levelezési profilok eltávolításáról a [levelezési beállítások felvétele a Intune segítségével](https://docs.microsoft.com/intune/email-settings-configure)című cikkben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="0dcf2-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="0dcf2-105">Ha további információra van kíváncsi a levelezési profilok létrehozásának módjáról, olvassa el az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="0dcf2-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="0dcf2-106">Az Android-eszközök beállításai az e-mailek, a hitelesítés és a szinkronizálás beállításához a Intune-ban</span><span class="sxs-lookup"><span data-stu-id="0dcf2-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="0dcf2-107">E-mail-beállítások megadása iOS-és iPadOS-eszközökhöz a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="0dcf2-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="0dcf2-108">A Microsoft Intune levelezési profil beállításai a Windows Phone 8,1 rendszerű eszközökön</span><span class="sxs-lookup"><span data-stu-id="0dcf2-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="0dcf2-109">A Microsoft Intune szolgáltatásban a Windows 10 rendszert futtató eszközök levelezési profiljának beállításai</span><span class="sxs-lookup"><span data-stu-id="0dcf2-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="0dcf2-110">**Gyakori szinkronizálási probléma**</span><span class="sxs-lookup"><span data-stu-id="0dcf2-110">**Common syncing issue**</span></span>

<span data-ttu-id="0dcf2-111">**A KNOX az Android-alapú e-mail-profilban megakadályozza a felhasználói partnereket, a naptárat és a feladatokat, illetve a felhasználói eszközök szinkronizálását.**</span><span class="sxs-lookup"><span data-stu-id="0dcf2-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="0dcf2-112">A KNOX az Android KNOX e-mail-profiljában lehetőséget nyújt a rendszergazda számára annak a beállításnak a megadására, hogy mely tartalomtípusok legyenek szinkronizálva az eszközre a minden beállítás engedélyezésével.</span><span class="sxs-lookup"><span data-stu-id="0dcf2-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="0dcf2-113">Ha a tartalomtípusok bármelyike beállítás értéke **nincs konfigurálva** (az alapértelmezett), a tartalomtípus nem szinkronizálódik automatikusan.</span><span class="sxs-lookup"><span data-stu-id="0dcf2-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="0dcf2-114">Előfordulhat, hogy egy felhasználó manuálisan engedélyezte azt a tartalomtípust, amelyet közvetlenül az eszközön szeretne használni, de az Intune házirend-beállítás felülírja az adott tartalomtípushoz tartozó szinkronizálási beállításokat.</span><span class="sxs-lookup"><span data-stu-id="0dcf2-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

