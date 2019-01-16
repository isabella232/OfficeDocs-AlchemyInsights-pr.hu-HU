---
title: Fájl megnyitása csak olvasásra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 69705825-723a-4c1e-ae85-d16b5051d2fe
ms.openlocfilehash: 45078e83f86f34386a7a2a2c0409f225122a598d
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293308"
---
# <a name="file-open-read-only"></a><span data-ttu-id="5308c-102">Fájl megnyitása csak olvasásra</span><span class="sxs-lookup"><span data-stu-id="5308c-102">File open read-only</span></span>

<span data-ttu-id="5308c-p101">Előfordulhat, hogy fájlok megnyitása, azok megnyitása csak olvasásra. Bizonyos esetekben ez a nagyobb biztonság, például a fájlok megnyitása az internetről, és máskor, azt okozhatja olyan beállítás, amely módosítható. Az alábbiakban azonban olyan helyzetek, amikor egy fájl nyílik meg, csak olvasható, és néhány lépést, módosíthatja, hogy is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="5308c-p101">You may find that when you are opening files, they open as read-only. In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed. Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="5308c-106">**Saját antivirus okozza azokat megnyitása csak olvasásra**</span><span class="sxs-lookup"><span data-stu-id="5308c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="5308c-p102">Egyes víruskereső programok is védve potenciálisan nem biztonságos fájlok megnyitásával őket csak olvasható. Szükség lehet érdeklődjön arról, hogy miként kell ezeket a beállításokat a víruskereső program szolgáltatójánál. BitDefender, például van itt alkalmazás kizárások hozzáadása tartalom: [alkalmazás vagy folyamat Bitdefender Control Center kizárások hozzáadása](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="5308c-p102">Some antivirus programs may protect you from potentially unsafe files by opening them read-only. You may need to check with your antivirus provider to learn how to adjust these settings. BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="5308c-110">**A fájl tulajdonságai megfelelőek-csak olvasható?**</span><span class="sxs-lookup"><span data-stu-id="5308c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="5308c-p103">Kattintson a jobb gombbal a fájlra, majd válassza a tulajdonságok is ellenőrizheti a fájl tulajdonságait. Ha az írásvédett attribútum be van jelölve, akkor törölje a bejelölést, és kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="5308c-p103">You can check the file properties by right-clicking on the file and choosing Properties. If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="5308c-113">**A tartalom védett nézetben van.**</span><span class="sxs-lookup"><span data-stu-id="5308c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="5308c-p104">Az internetről és más potenciálisan nem biztonságos helyről fájlok is tartalmazhatnak, vírusok, férgek vagy egyéb rosszindulatú programok, amelyek kárt okozhatnak a számítógépben. Ez helyzet is gyakran az e-mail mellékletek vagy a letöltött fájlokat. A számítógép védelme érdekében, hogy ezeken a helyeken potenciálisan nem biztonságos fájlokat védett nézetben nyitja meg. A védett nézet olvasni a fájlt és annak tartalmát megtekintheti a kockázatok mérséklését. További információt a védett megtekintése és módosítása, lásd a cikk: [Mi az a védett nézet?](https://support.office.com/en-us/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="5308c-p104">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer. This is also commonly the case with email attachments or files you've downloaded. To help protect your computer, files from these potentially unsafe locations are opened in Protected View. By using Protected View, you can read a file and see its contents while reducing the risks. For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/en-us/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="5308c-119">**Tele van a OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="5308c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="5308c-p105">Ha a fájl található a OneDrive és a OneDrive tárolási hely megtelt, tudják, mentse a dokumentumot, amíg az erre szánt terület mellett. Ellenőrizheti a OneDrive lévő szabad terület értesítési közepén lévő OneDrive ikonra kattintva, majd válassza a kezelés, tárolás, vagy nyissa meg [http://onedrive.live.com](http://onedrive.live.com), jelentkezzen be, és jegyezze fel a képernyő bal alsó használt terület nagysága.</span><span class="sxs-lookup"><span data-stu-id="5308c-p105">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space. You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="5308c-122">**Office aktiválva van?**</span><span class="sxs-lookup"><span data-stu-id="5308c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="5308c-p106">Ha Office nincs aktiválva, vagy az előfizetése lejárt, akkor lehet csak olvasható csökkentett módban. Olvashat az Office Aktiválás, lásd: [nem licencelt termék és az Office Aktiválás hibákat](https://support.office.com/en-us/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="5308c-p106">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode. For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/en-us/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="5308c-125">**Ha más nem segít...**</span><span class="sxs-lookup"><span data-stu-id="5308c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="5308c-126">Próbálja meg újraindítani a számítógépet</span><span class="sxs-lookup"><span data-stu-id="5308c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="5308c-127">Az Office-frissítések telepítése</span><span class="sxs-lookup"><span data-stu-id="5308c-127">Install Office updates</span></span>
    
- <span data-ttu-id="5308c-128">Hajtsa végre az Office Online javítása</span><span class="sxs-lookup"><span data-stu-id="5308c-128">Perform an Online repair of Office</span></span>
    

