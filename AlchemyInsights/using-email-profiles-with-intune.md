---
title: E-mail profilok használata az Intune-nal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555254"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="22122-102">E-mail profilok használata az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="22122-102">Using email profiles with Intune</span></span>

<span data-ttu-id="22122-103">Az Intune segítségével több eszközön is létrehozhat és üzembe helyezhet e-mail-profilokat a natív (beépített) levelezőprogramhoz.</span><span class="sxs-lookup"><span data-stu-id="22122-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="22122-104">Az e-mail profilokhoz kapcsolódó korlátozásokról, beleértve a meglévő profilok jelenlétének kezelését és az e-mail profilok eltávolításának módját, az [E-mail beállítások hozzáadása az Intune használatával című témakörben](https://docs.microsoft.com/intune/email-settings-configure)olvashat.</span><span class="sxs-lookup"><span data-stu-id="22122-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="22122-105">Az egyes eszközplatformokhoz az e-mail profilok létrehozásáról az:</span><span class="sxs-lookup"><span data-stu-id="22122-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="22122-106">Android-eszközbeállítások az e-mailek, a hitelesítés és a szinkronizálás konfigurálásához az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="22122-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="22122-107">E-mail beállítások hozzáadása iOS- és iPadOS-eszközökhöz a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="22122-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="22122-108">E-mail profil beállítások a Microsoft Intune-ban Windows Phone 8.1-es rendszerű eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="22122-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="22122-109">E-mail profil beállítások a Microsoft Intune-ban windows 10-et futtató eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="22122-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="22122-110">**Gyakori szinkronizálási probléma**</span><span class="sxs-lookup"><span data-stu-id="22122-110">**Common syncing issue**</span></span>

<span data-ttu-id="22122-111">**Az Android-alapú KNOX e-mail-profil megakadályozza, hogy a felhasználói névjegyek, a naptár és a feladatok szinkronizálódjanak a felhasználói eszközökkel.**</span><span class="sxs-lookup"><span data-stu-id="22122-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="22122-112">A KNOX on Android KNOX e-mail profil lehetővé teszi a rendszergazda számára annak eldöntését, hogy mely tartalomtípusok vannak szinkronizálva az eszközre, ha az egyes eket engedélyezi.</span><span class="sxs-lookup"><span data-stu-id="22122-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="22122-113">Ha bármelyik tartalomtípus beállítása **Nincs konfigurálva** (ez az alapértelmezett), akkor az adott tartalomtípus nem lesz automatikusan szinkronizálva.</span><span class="sxs-lookup"><span data-stu-id="22122-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="22122-114">Előfordulhat, hogy a felhasználó manuálisan engedélyezi a kívánt tartalomtípust az eszközön, de ezt a konfigurációt az Intune házirend-beállítása felülírja, és az adott tartalomtípus szinkronizálása leáll.</span><span class="sxs-lookup"><span data-stu-id="22122-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

