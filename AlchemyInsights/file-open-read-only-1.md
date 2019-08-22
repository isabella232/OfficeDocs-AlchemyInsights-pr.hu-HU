---
title: Fájl megnyitása csak olvasásra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 69705825-723a-4c1e-ae85-d16b5051d2fe
ms.openlocfilehash: 06c052383a6462288270d2e062930352883a199a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525712"
---
# <a name="file-open-read-only"></a><span data-ttu-id="1abc7-102">Fájl megnyitása csak olvasásra</span><span class="sxs-lookup"><span data-stu-id="1abc7-102">File open read-only</span></span>

<span data-ttu-id="1abc7-103">Előfordulhat, hogy fájlok megnyitása, azok megnyitása csak olvasásra.</span><span class="sxs-lookup"><span data-stu-id="1abc7-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="1abc7-104">Bizonyos esetekben ez a nagyobb biztonság, például a fájlok megnyitása az internetről, és máskor, azt okozhatja olyan beállítás, amely módosítható.</span><span class="sxs-lookup"><span data-stu-id="1abc7-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="1abc7-105">Az alábbiakban azonban olyan helyzetek, amikor egy fájl nyílik meg, csak olvasható, és néhány lépést, módosíthatja, hogy is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="1abc7-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="1abc7-106">**Saját antivirus okozza azokat megnyitása csak olvasásra**</span><span class="sxs-lookup"><span data-stu-id="1abc7-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="1abc7-107">Egyes víruskereső programok is védve potenciálisan nem biztonságos fájlok megnyitásával őket csak olvasható.</span><span class="sxs-lookup"><span data-stu-id="1abc7-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="1abc7-108">Szükség lehet érdeklődjön arról, hogy miként kell ezeket a beállításokat a víruskereső program szolgáltatójánál.</span><span class="sxs-lookup"><span data-stu-id="1abc7-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="1abc7-109">BitDefender, például van itt alkalmazás kizárások hozzáadása tartalom: [alkalmazás vagy folyamat Bitdefender Control Center kizárások hozzáadása](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="1abc7-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="1abc7-110">**A fájl tulajdonságai megfelelőek-csak olvasható?**</span><span class="sxs-lookup"><span data-stu-id="1abc7-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="1abc7-111">Kattintson a jobb gombbal a fájlra, majd válassza a tulajdonságok is ellenőrizheti a fájl tulajdonságait.</span><span class="sxs-lookup"><span data-stu-id="1abc7-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="1abc7-112">Ha az írásvédett attribútum be van jelölve, akkor törölje a bejelölést, és kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="1abc7-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="1abc7-113">**A tartalom védett nézetben van.**</span><span class="sxs-lookup"><span data-stu-id="1abc7-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="1abc7-114">Az internetről és más potenciálisan nem biztonságos helyről fájlok is tartalmazhatnak, vírusok, férgek vagy egyéb rosszindulatú programok, amelyek kárt okozhatnak a számítógépben.</span><span class="sxs-lookup"><span data-stu-id="1abc7-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="1abc7-115">Ez helyzet is gyakran az e-mail mellékletek vagy a letöltött fájlokat.</span><span class="sxs-lookup"><span data-stu-id="1abc7-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="1abc7-116">A számítógép védelme érdekében, hogy ezeken a helyeken potenciálisan nem biztonságos fájlokat védett nézetben nyitja meg.</span><span class="sxs-lookup"><span data-stu-id="1abc7-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="1abc7-117">A védett nézet olvasni a fájlt és annak tartalmát megtekintheti a kockázatok mérséklését.</span><span class="sxs-lookup"><span data-stu-id="1abc7-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="1abc7-118">További információt a védett megtekintése és módosítása, lásd a cikk: [Mi az a védett nézet?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="1abc7-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="1abc7-119">**Tele van a OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="1abc7-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="1abc7-120">Ha a fájl található a OneDrive és a OneDrive tárolási hely megtelt, tudják, mentse a dokumentumot, amíg az erre szánt terület mellett.</span><span class="sxs-lookup"><span data-stu-id="1abc7-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="1abc7-121">Ellenőrizheti a OneDrive lévő szabad terület értesítési közepén lévő OneDrive ikonra kattintva, majd válassza a kezelés, tárolás, vagy nyissa meg [http://onedrive.live.com](http://onedrive.live.com), jelentkezzen be, és jegyezze fel a képernyő bal alsó használt terület nagysága.</span><span class="sxs-lookup"><span data-stu-id="1abc7-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="1abc7-122">**Office aktiválva van?**</span><span class="sxs-lookup"><span data-stu-id="1abc7-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="1abc7-123">Ha Office nincs aktiválva, vagy az előfizetése lejárt, akkor lehet csak olvasható csökkentett módban.</span><span class="sxs-lookup"><span data-stu-id="1abc7-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="1abc7-124">Olvashat az Office Aktiválás, lásd: [nem licencelt termék és az Office Aktiválás hibákat](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="1abc7-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="1abc7-125">**Ha más nem segít...**</span><span class="sxs-lookup"><span data-stu-id="1abc7-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="1abc7-126">Próbálja meg újraindítani a számítógépet</span><span class="sxs-lookup"><span data-stu-id="1abc7-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="1abc7-127">Az Office-frissítések telepítése</span><span class="sxs-lookup"><span data-stu-id="1abc7-127">Install Office updates</span></span>
    
- <span data-ttu-id="1abc7-128">Hajtsa végre az Office Online javítása</span><span class="sxs-lookup"><span data-stu-id="1abc7-128">Perform an Online repair of Office</span></span>
    

