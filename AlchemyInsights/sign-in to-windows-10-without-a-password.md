---
title: Bejelentkezés a Windows 10-be jelszó használata nélkül
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588283"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="cd6d8-102">Bejelentkezés a Windows 10-be jelszó használata nélkül</span><span class="sxs-lookup"><span data-stu-id="cd6d8-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="cd6d8-103">Annak elkerülése érdekében, hogy a Windows indításakor jelszót kelljen beírnia, javasoljuk, hogy használja a Windows Hello biztonságos bejelentkezési beállításainak egyikét, például pin-kódot, arcfelismerést vagy ujjlenyomatot, ha van ilyen.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="cd6d8-104">Ha valóban le szeretné tiltani a biztonságos bejelentkezést, olvassa el az alábbi, "Automatikus bejelentkezés a Windows 10-be" című útmutatót.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="cd6d8-105">**Biztonságos Windows Hello alternatívái a fiók jelszavához**</span><span class="sxs-lookup"><span data-stu-id="cd6d8-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="cd6d8-106">Nyissa meg a **Beállítások > fiókok > bejelentkezési beállításokat** (vagy kattintson [ide](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="cd6d8-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="cd6d8-107">Az elérhető bejelentkezési lehetőségek megjelennek a listában.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="cd6d8-108">Például:</span><span class="sxs-lookup"><span data-stu-id="cd6d8-108">For example:</span></span>

![Bejelentkezési beállítások.](media/sign-in-options.png)

<span data-ttu-id="cd6d8-110">A konfiguráláshoz kattintson vagy koppintson az egyik beállítási lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="cd6d8-111">A Windows indításakor vagy zárolásának feloldásakor jelszó helyett az új opciót használhatja.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="cd6d8-112">**Automatikus bejelentkezés a Windows 10-be**</span><span class="sxs-lookup"><span data-stu-id="cd6d8-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="cd6d8-113">**Megjegyzés:** Az automatikus bejelentkezés kényelmes, de biztonsági kockázatot jelent, különösen akkor, ha a számítógép több ember számára is elérhető.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="cd6d8-114">Kattintson vagy koppintson a **Tálca Start** gombjára.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="cd6d8-115">Írja be a **netplwiz parancsot,** és nyomja meg az Enter billentyűt a Felhasználói fiókok ablak megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="cd6d8-116">A **Felhasználói fiókok**csoportban kattintson arra a fiókra, amelybe a Windows indításakor automatikusan be szeretne jelentkezni.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="cd6d8-117">Törölje a jelet a "A számítógép használatához a felhasználóknak meg kell adnia egy felhasználónevet és jelszót" jelölőnégyzetjelölését.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![A felhasználóknak meg kell adniuk egy felhasználónevet és jelszót.](media/users-must-enter-username.png)

5. <span data-ttu-id="cd6d8-119">Kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-119">Click **OK**.</span></span> <span data-ttu-id="cd6d8-120">A rendszer megkéri, hogy adja meg és erősítse meg a kiválasztott fiók jelszavát.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="cd6d8-121">A befejezéshez kattintson az **OK** gombra.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-121">Click **OK** to finish.</span></span> <span data-ttu-id="cd6d8-122">A Windows 10 következő indításakor automatikusan bejelentkezik a kiválasztott fiókba.</span><span class="sxs-lookup"><span data-stu-id="cd6d8-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
