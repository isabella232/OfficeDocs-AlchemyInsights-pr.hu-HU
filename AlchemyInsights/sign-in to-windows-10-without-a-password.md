---
title: Bejelentkezés a Windows 10-es verzióba jelszó használata nélkül
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719955"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="78c07-102">Bejelentkezés a Windows 10-es verzióba jelszó használata nélkül</span><span class="sxs-lookup"><span data-stu-id="78c07-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="78c07-103">Ha nem szeretne jelszót beírni a Windows indításakor, azt javasoljuk, hogy használja a Windows Hello Secure bejelentkezési beállításait, például a PIN-kódot, az Arcfelismerés vagy az ujjlenyomatot, ha van ilyen.</span><span class="sxs-lookup"><span data-stu-id="78c07-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="78c07-104">Ha valóban le szeretné tiltani a biztonságos bejelentkezést, olvassa el az alábbi utasításokat az automatikus bejelentkezés a Windows 10-es verzióba című témakörben.</span><span class="sxs-lookup"><span data-stu-id="78c07-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="78c07-105">**A Windows Hello alternatívái a fiók jelszavának védelme**</span><span class="sxs-lookup"><span data-stu-id="78c07-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="78c07-106">Lépjen a **beállítások >-fiókok > bejelentkezési beállítások** elemre (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="78c07-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="78c07-107">A rendelkezésre álló bejelentkezési beállítások megjelennek.</span><span class="sxs-lookup"><span data-stu-id="78c07-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="78c07-108">Például:</span><span class="sxs-lookup"><span data-stu-id="78c07-108">For example:</span></span>

![Bejelentkezési lehetőségek](media/sign-in-options.png)

<span data-ttu-id="78c07-110">Kattintson vagy koppintson az egyik lehetőségre a beállításához.</span><span class="sxs-lookup"><span data-stu-id="78c07-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="78c07-111">A Windows következő indításakor vagy zárolásának feloldásakor a jelszó helyett az új lehetőséget fogja használni.</span><span class="sxs-lookup"><span data-stu-id="78c07-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="78c07-112">**Automatikus bejelentkezés a Windows 10-es verzióba**</span><span class="sxs-lookup"><span data-stu-id="78c07-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="78c07-113">**Megjegyzés**: az automatikus bejelentkezés kényelmes, de biztonsági kockázatot jelent, különösen akkor, ha a számítógépe több személy számára is elérhető.</span><span class="sxs-lookup"><span data-stu-id="78c07-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="78c07-114">Kattintson vagy koppintson a **Start** gombra a tálcán.</span><span class="sxs-lookup"><span data-stu-id="78c07-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="78c07-115">Írja be a **netplwiz** , és az ENTER billentyűt lenyomva nyissa meg a felhasználói fiókok ablakot.</span><span class="sxs-lookup"><span data-stu-id="78c07-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="78c07-116">A **felhasználói fiókokban**kattintson arra a fiókra, amellyel a Windows indításakor automatikusan be szeretne jelentkezne.</span><span class="sxs-lookup"><span data-stu-id="78c07-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="78c07-117">Törölje a jelet a "felhasználóknak meg kell adni a felhasználónevet és a jelszót a számítógép használatához" jelölőnégyzetből.</span><span class="sxs-lookup"><span data-stu-id="78c07-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![A felhasználóknak meg kell adni a Felhasználónév és a jelszó beállítást.](media/users-must-enter-username.png)

5. <span data-ttu-id="78c07-119">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="78c07-119">Click **OK**.</span></span> <span data-ttu-id="78c07-120">A rendszer kérni fogja a kijelölt fiók jelszavának megadását és megerősítését.</span><span class="sxs-lookup"><span data-stu-id="78c07-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="78c07-121">A befejezéshez kattintson **az OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="78c07-121">Click **OK** to finish.</span></span> <span data-ttu-id="78c07-122">A Windows 10 következő indításakor a program automatikusan bejelentkezik a kijelölt fiókba.</span><span class="sxs-lookup"><span data-stu-id="78c07-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
