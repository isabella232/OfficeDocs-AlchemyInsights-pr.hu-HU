---
title: A fájl írásvédett
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: c045188af15fcec0f868eb0e5b399bd1fb42a09a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702776"
---
# <a name="file-open-read-only"></a><span data-ttu-id="a9d9e-102">A fájl írásvédett</span><span class="sxs-lookup"><span data-stu-id="a9d9e-102">File open read-only</span></span>

<span data-ttu-id="a9d9e-103">Előfordulhat, hogy a fájlok megnyitásakor azok írásvédettként nyílnak meg.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="a9d9e-104">Bizonyos esetekben ez a nagyobb biztonság érdekében történik, például amikor fájlokat nyit meg az internetről, máskor pedig egy módosítható beállításnak lehet az oka.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="a9d9e-105">Íme néhány forgatókönyv, amikor egy fájl írásvédett, és néhány lépéssel módosíthatja ezt.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="a9d9e-106">**A víruskereső miatt csak olvasásra van nyitva**</span><span class="sxs-lookup"><span data-stu-id="a9d9e-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="a9d9e-107">Egyes víruskereső programok írásvédett megnyitásával megvédhetik Önt a potenciálisan nem biztonságos fájloktól.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="a9d9e-108">Előfordulhat, hogy a beállítások módosításáról érdeklődjön a víruskereső szolgáltatójánál.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="a9d9e-109">BitDefender, például, van tartalom hozzáadásával alkalmazás kizárások itt: [Hogyan adjunk alkalmazás vagy folyamat kizárások Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="a9d9e-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="a9d9e-110">**A fájltulajdonságok írásvédettre vannak állítva?**</span><span class="sxs-lookup"><span data-stu-id="a9d9e-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="a9d9e-111">A fájl tulajdonságait úgy ellenőrizheti, hogy a jobb gombbal a fájlra kattint, és a Tulajdonságok parancsot választja.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="a9d9e-112">Ha az Írásvédett attribútum be van jelölve, törölje a jelet, és kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="a9d9e-113">**A tartalom védett nézetben van**</span><span class="sxs-lookup"><span data-stu-id="a9d9e-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="a9d9e-114">Az internetről és más, potenciálisan nem biztonságos helyekről származó fájlok vírusokat, férgeket vagy más rosszindulatú programokat tartalmazhatnak, amelyek károsíthatják a számítógépet.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="a9d9e-115">Ez gyakran előfordul az e-mail mellékletekkel vagy a letöltött fájlokkal is.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="a9d9e-116">A számítógép védelme érdekében az ilyen potenciálisan nem biztonságos helyekről származó fájlok védett nézetben nyílnak meg.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="a9d9e-117">A Védett nézet használatával elolvashatja a fájlokat, és megtekintheti annak tartalmát, miközben csökkenti a kockázatokat.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="a9d9e-118">A védett nézetről és a beállítások módosításáról a következő cikkben olvashat: [Mi a védett nézet?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="a9d9e-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="a9d9e-119">**Megtelt a OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="a9d9e-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="a9d9e-120">Ha a fájl a OneDrive-on van tárolva, és a OneDrive tárhelye megtelt, addig nem tudja menteni a dokumentumot, amíg a megadott terület alatt nem van.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="a9d9e-121">A OneDrive-on a OneDrive-on lévő szabad területet az értesítési központban lévő OneDrive ikonra kattintva ellenőrizheti, és a Tárhely kezelése lehetőséget választja, vagy a , [https://onedrive.live.com](https://onedrive.live.com)bejelentkezhet, és feljegyzheti a képernyő bal alsó részén található felhasznált terület nagy részét.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="a9d9e-122">**Aktiválva van az Office?**</span><span class="sxs-lookup"><span data-stu-id="a9d9e-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="a9d9e-123">Ha az Office nincs aktiválva, vagy az előfizetése lejárt, akkor írásvédett csökkentett üzemmódban lehet.</span><span class="sxs-lookup"><span data-stu-id="a9d9e-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="a9d9e-124">Az Office aktiválásáról a Következő témakörben talál információt: [Nem licencelt termék és aktiválási hibák az Office-ban.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="a9d9e-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="a9d9e-125">**Ha minden más elbukik...**</span><span class="sxs-lookup"><span data-stu-id="a9d9e-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="a9d9e-126">Próbálja meg újraindítani a számítógépet</span><span class="sxs-lookup"><span data-stu-id="a9d9e-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="a9d9e-127">Office-frissítések telepítése</span><span class="sxs-lookup"><span data-stu-id="a9d9e-127">Install Office updates</span></span>
    
- <span data-ttu-id="a9d9e-128">Office online javításának végrehajtása</span><span class="sxs-lookup"><span data-stu-id="a9d9e-128">Perform an Online repair of Office</span></span>
    

