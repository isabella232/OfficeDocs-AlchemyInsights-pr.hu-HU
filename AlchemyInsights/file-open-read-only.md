---
title: Fájl megnyitása írásvédett
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745587"
---
# <a name="file-open-read-only"></a><span data-ttu-id="053ce-102">Fájl megnyitása írásvédett</span><span class="sxs-lookup"><span data-stu-id="053ce-102">File open read-only</span></span>

<span data-ttu-id="053ce-103">Előfordulhat, hogy a fájlok megnyitásakor csak olvashatóként nyílik meg.</span><span class="sxs-lookup"><span data-stu-id="053ce-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="053ce-104">Bizonyos esetekben ez a biztonság, például a fájlok internetről való megnyitásakor, illetve máskor is előfordulhat, hogy ez a beállítás a módosítható beállításnak köszönhető.</span><span class="sxs-lookup"><span data-stu-id="053ce-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="053ce-105">Íme néhány példa arra, hogy egy fájl írásvédett módban nyílik meg, és néhány lépésben megteheti a módosítást.</span><span class="sxs-lookup"><span data-stu-id="053ce-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="053ce-106">**A víruskeresők azt okozzák, hogy csak írásvédett módban nyílnak meg**</span><span class="sxs-lookup"><span data-stu-id="053ce-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="053ce-107">Egyes víruskereső programok csak olvashatóan tudják megvédeni a fájlokat a potenciálisan nem biztonságos fájlokból.</span><span class="sxs-lookup"><span data-stu-id="053ce-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="053ce-108">Ha meg szeretné tudni, hogy miként igazíthatja ezeket a beállításokat, előfordulhat, hogy meg kell vizsgálnia a víruskereső szolgáltatóját.</span><span class="sxs-lookup"><span data-stu-id="053ce-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="053ce-109">BitDefender (például) tartalma az alkalmazások kivételének hozzáadásához: [Hogyan vehet fel alkalmazást vagy folyamat kizárását a BitDefender Control Center alkalmazásban](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="053ce-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="053ce-110">**A fájl tulajdonságai csak olvashatók legyenek?**</span><span class="sxs-lookup"><span data-stu-id="053ce-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="053ce-111">A fájl tulajdonságainak ellenőrzéséhez kattintson a jobb gombbal a fájlra, és válassza a Tulajdonságok parancsot.</span><span class="sxs-lookup"><span data-stu-id="053ce-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="053ce-112">Ha a írásvédett attribútum be van jelölve, akkor törölje a jelet, és kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="053ce-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="053ce-113">**A tartalom védett nézetben van**</span><span class="sxs-lookup"><span data-stu-id="053ce-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="053ce-114">Az internetről és más, esetleg nem biztonságos helyekről származó fájlok tartalmazhatnak vírusokat, férgeket vagy más típusú kártevőket, amelyek károsíthatják a számítógépre.</span><span class="sxs-lookup"><span data-stu-id="053ce-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="053ce-115">Ez a helyzet általában az e-mail-mellékletek vagy a letöltött fájlok esetén is.</span><span class="sxs-lookup"><span data-stu-id="053ce-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="053ce-116">A számítógép védelme érdekében a nem biztonságos helyekről származó fájlok védett nézetben nyílnak meg.</span><span class="sxs-lookup"><span data-stu-id="053ce-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="053ce-117">A védett nézet használatával elolvashatja a fájlt, és megtekintheti a tartalmát, miközben csökkenti a kockázatokat.</span><span class="sxs-lookup"><span data-stu-id="053ce-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="053ce-118">A védett nézetről és a beállítások módosításáról a [védett nézet](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653) című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="053ce-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="053ce-119">**Teljes a OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="053ce-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="053ce-120">Ha a fájl a OneDrive van tárolva, és a OneDrive tárterülete megtelik, akkor a program nem menti a dokumentumot, amíg el nem éri a kiosztott tárterületét.</span><span class="sxs-lookup"><span data-stu-id="053ce-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="053ce-121">Az OneDrive-on lévő szabad terület ellenőrzéséhez kattintson a OneDrive ikonra az értesítési központban, és válassza a tárterület kezelése lehetőséget, vagy lépjen a [https://onedrive.live.com](https://onedrive.live.com) képernyő bal alsó részén lévő szabad területhez.</span><span class="sxs-lookup"><span data-stu-id="053ce-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="053ce-122">**Aktivált az Office?**</span><span class="sxs-lookup"><span data-stu-id="053ce-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="053ce-123">Ha az Office nincs aktiválva, vagy lejárt az előfizetése, akkor csak olvasható csökkentett módban lehet.</span><span class="sxs-lookup"><span data-stu-id="053ce-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="053ce-124">Az Office aktiválásához további információt a következő témakörben talál: nem [licencelt termék-és aktiválási hibák az Office-ban](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="053ce-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="053ce-125">**Ha minden kötél szakadt meg...**</span><span class="sxs-lookup"><span data-stu-id="053ce-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="053ce-126">Próbálkozzon a számítógép újraindításával</span><span class="sxs-lookup"><span data-stu-id="053ce-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="053ce-127">Office-frissítések telepítése</span><span class="sxs-lookup"><span data-stu-id="053ce-127">Install Office updates</span></span>
    
- <span data-ttu-id="053ce-128">Az Office Online javításának elvégzése</span><span class="sxs-lookup"><span data-stu-id="053ce-128">Perform an Online repair of Office</span></span>
    

