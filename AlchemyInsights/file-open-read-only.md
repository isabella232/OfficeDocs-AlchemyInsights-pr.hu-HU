---
title: Fájlmegnyitás csak olvasásra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: eddd427b159a782abf53adda934de8b15a02ed00
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822236"
---
# <a name="file-open-read-only"></a><span data-ttu-id="1927b-102">Fájlmegnyitás csak olvasásra</span><span class="sxs-lookup"><span data-stu-id="1927b-102">File open read-only</span></span>

<span data-ttu-id="1927b-103">Előfordulhat, hogy a fájlok megnyitásakor csak olvasottként jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="1927b-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="1927b-104">Bizonyos esetekben ez a további biztonság, például a fájlok internetről való megnyitásakor, máskor is fontos, lehet, hogy egy módosítható beállítás is köszönhető.</span><span class="sxs-lookup"><span data-stu-id="1927b-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="1927b-105">Az alábbiakban néhány olyan esetet talál, amikor egy fájl csak olvasásra nyílik meg, és néhány lépést megtehet annak módosításához.</span><span class="sxs-lookup"><span data-stu-id="1927b-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="1927b-106">**Saját víruskereső okozza, hogy megnyitja csak olvasható**</span><span class="sxs-lookup"><span data-stu-id="1927b-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="1927b-107">Egyes víruskereső programok a potenciálisan veszélyes fájlokon védelmet is nyújthat, ha azokat csak olvasásra nyitja meg.</span><span class="sxs-lookup"><span data-stu-id="1927b-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="1927b-108">Előfordulhat, hogy meg kell keresnia a víruskereső program szolgáltatóját, hogy megtudja, hogyan módosíthatja ezeket a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="1927b-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="1927b-109">BitDefender, például, birtokol elégedett-ra összeadás alkalmazás kizárás itt: [Hogyan viselkedni összead alkalmazás vagy folyamat kizárás-ban BitDefender irányít központ](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="1927b-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="1927b-110">**A fájltulajdonságok csak olvasásra vannak beállítva?**</span><span class="sxs-lookup"><span data-stu-id="1927b-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="1927b-111">A fájltulajdonságok ellenőrzéséhez kattintson jobb gombbal a fájlra, és válassza a Tulajdonságok parancsot.</span><span class="sxs-lookup"><span data-stu-id="1927b-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="1927b-112">Ha az írásvédett attribútum van bejelölve, akkor törölje a bejelölést, és kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="1927b-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="1927b-113">**A tartalom védett nézetben van**</span><span class="sxs-lookup"><span data-stu-id="1927b-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="1927b-114">Az internetről és más, potenciálisan veszélyes helyekről származó fájlok vírusokat, férgeket vagy más, a számítógépet károsító kártevőket tartalmazhatnak.</span><span class="sxs-lookup"><span data-stu-id="1927b-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="1927b-115">Ez is általában a helyzet-val elektronikus levél egybefűzés vagy fájlokat youve ' letöltött.</span><span class="sxs-lookup"><span data-stu-id="1927b-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="1927b-116">A számítógép védelme érdekében az ilyen, potenciálisan veszélyes helyekről származó fájlokat a védett nézet nyitja meg.</span><span class="sxs-lookup"><span data-stu-id="1927b-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="1927b-117">A védett nézet használatával egy fájl elolvasható, és tartalma a kockázatok csökkentése mellett látható.</span><span class="sxs-lookup"><span data-stu-id="1927b-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="1927b-118">A védett nézetről és a beállítások módosítására vonatkozó további információ a következő cikkben található: [Mi a védett nézet?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="1927b-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="1927b-119">**A OneDrive teljes?**</span><span class="sxs-lookup"><span data-stu-id="1927b-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="1927b-120">Ha a fájl tárolása a OneDrive és az OneDrive tárterület megtelt, akkor nem tudja menteni a dokumentumot, amíg nem a kiosztott hely.</span><span class="sxs-lookup"><span data-stu-id="1927b-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="1927b-121">Akkor ellenőrizze a szabad hely OneDrive kattintva az OneDrive ikonra az értesítési központban, és válassza a tárolás kezelése, vagy mehetsz [http://onedrive.live.com](http://onedrive.live.com), jelentkezzen be, és jegyezze meg a felhasznált terület a bal alsó sarkában a képernyőn.</span><span class="sxs-lookup"><span data-stu-id="1927b-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="1927b-122">**Aktiválva van az Office?**</span><span class="sxs-lookup"><span data-stu-id="1927b-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="1927b-123">Ha az Office nincs aktiválva, vagy ha az előfizetés lejárt, csak olvasási üzemmódban lehet csökkentett szolgáltatáskészletet nyújtó módban.</span><span class="sxs-lookup"><span data-stu-id="1927b-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="1927b-124">Az Office aktiválásához lásd: [licenc nélküli termék-és aktiválási hibák az Office-ban](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="1927b-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="1927b-125">**Ha minden kötél szakad...**</span><span class="sxs-lookup"><span data-stu-id="1927b-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="1927b-126">Próbálkozzon a számítógép újraindításával.</span><span class="sxs-lookup"><span data-stu-id="1927b-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="1927b-127">Az Office-frissítések telepítése</span><span class="sxs-lookup"><span data-stu-id="1927b-127">Install Office updates</span></span>
    
- <span data-ttu-id="1927b-128">Előad egy online kijavít-ból Hivatal</span><span class="sxs-lookup"><span data-stu-id="1927b-128">Perform an Online repair of Office</span></span>
    

