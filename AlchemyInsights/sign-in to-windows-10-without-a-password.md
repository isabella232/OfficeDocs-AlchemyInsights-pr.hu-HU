---
title: Bejelentkezés a Windows 10-be jelszó használata nélkül
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830548"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="8cb6e-102">Bejelentkezés a Windows 10-be jelszó használata nélkül</span><span class="sxs-lookup"><span data-stu-id="8cb6e-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="8cb6e-103">Ha el szeretné kerülni, hogy jelszót kelljen megadnia a Windows rendszer indításakor, javasoljuk, hogy használja a Windows Hello biztonságos bejelentkezési beállításait, például PIN-kódot, arcfelismerést vagy ujjlenyomatot, ha van ilyen.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="8cb6e-104">Ha valóban le szeretné tiltani a biztonságos bejelentkezést, olvassa el alább az "Automatikus bejelentkezés a Windows 10-be" utasításokat.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="8cb6e-105">**A fiókjelszó alternatívái a Windows Hello biztonságos használata esetén**</span><span class="sxs-lookup"><span data-stu-id="8cb6e-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="8cb6e-106">Válassza **a Beállítások > Fiókok > Bejelentkezési** lehetőségek lehetőséget (vagy kattintson [ide).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="8cb6e-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="8cb6e-107">Az elérhető bejelentkezési lehetőségek listája megjelenik.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="8cb6e-108">Például:</span><span class="sxs-lookup"><span data-stu-id="8cb6e-108">For example:</span></span>

![Bejelentkezési lehetőségek.](media/sign-in-options.png)

<span data-ttu-id="8cb6e-110">A beállításhoz kattintson vagy koppintson az egyik beállításra.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="8cb6e-111">Amikor legközelebb elindítja vagy feloldja a Windows zárolását, jelszó helyett használhatja az új beállítást.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="8cb6e-112">**Automatikus bejelentkezés a Windows 10-be**</span><span class="sxs-lookup"><span data-stu-id="8cb6e-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="8cb6e-113">**Megjegyzés:** Az automatikus bejelentkezés kényelmes, de biztonsági kockázatot jelent, különösen akkor, ha a számítógép több felhasználó számára is elérhető.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="8cb6e-114">Kattintson vagy koppintson a **Start** gombra a tálcán.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="8cb6e-115">Írja **be a netplwiz parancsot,** és nyomja le az Enter billentyűt a Felhasználói fiókok ablak megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="8cb6e-116">A **Felhasználói fiókok csoportban** kattintson arra a fiókra, amelybe automatikusan be szeretne jelentkezni a Windows indításakor.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="8cb6e-117">Törölje "A felhasználóknak meg kell adnia egy felhasználónevet és jelszót a számítógép használatához" jelölőnégyzet jelölését.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![A felhasználóknak meg kell adnia a felhasználónevet és a jelszót.](media/users-must-enter-username.png)

5. <span data-ttu-id="8cb6e-119">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-119">Click **OK**.</span></span> <span data-ttu-id="8cb6e-120">A program kérni fogja, hogy adja meg és erősítse meg a kijelölt fiók jelszavát.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="8cb6e-121">A **befejezéshez kattintson** az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-121">Click **OK** to finish.</span></span> <span data-ttu-id="8cb6e-122">A Windows 10 következő indításakor a rendszer automatikusan bejelentkezik a kiválasztott fiókba.</span><span class="sxs-lookup"><span data-stu-id="8cb6e-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
