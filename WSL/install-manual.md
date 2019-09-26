---
title: Manuelles Herunterladen von Windows-Subsystem für Linux (WSL)
description: Anweisungen zum manuellen Herunterladen des Windows-Subsystems für Linux-Distributionen.
keywords: Bashonwindows, bash, WSL, Windows, Windows-Subsystem für Linux, WSL, Windows-Subsystem, Distribution, Ubuntu, openSUSE, SLES, Debian, Kali
ms.date: 07/24/2018
ms.topic: article
ms.assetid: 9281ffa2-4fa9-4078-bf6f-b51c967617e3
ms.custom: seodec18
ms.openlocfilehash: df47e656cf83e0b13aa8eb3f210e010d6a85bfd8
ms.sourcegitcommit: 0b5a9f8982dfff07fc8df32d74d97293654f8e12
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2019
ms.locfileid: "71269790"
---
# <a name="manually-download-windows-subsystem-for-linux-distro-packages"></a><span data-ttu-id="26d5e-104">Manuelles Herunterladen von Windows-Subsystem für Linux-Distribution-Pakete</span><span class="sxs-lookup"><span data-stu-id="26d5e-104">Manually download Windows Subsystem for Linux distro packages</span></span>

<span data-ttu-id="26d5e-105">Es gibt mehrere Szenarios, in denen Sie möglicherweise nicht in der Lage sind, WSL-Linux-Distributionen über die Microsoft Store zu installieren (oder möchten).</span><span class="sxs-lookup"><span data-stu-id="26d5e-105">There are several scenarios in which you may not be able (or want) to, install WSL Linux distros via the Microsoft Store.</span></span> <span data-ttu-id="26d5e-106">Vor allem können Sie eine Windows Server-oder eine LTSC-Desktop-SKU (Long-Term Wartung) ausführen, die keine Microsoft Store unterstützt, oder Ihre Unternehmensnetzwerk Richtlinien und/oder Administratoren, um die Verwendung von Microsoft Store in Ihrer Umgebung nicht zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="26d5e-106">Specifically, you may be running a Windows Server or Long-Term Servicing (LTSC) desktop OS SKU that doesn't support Microsoft Store, or your corporate network policies and/or admins to not permit Microsoft Store usage in your environment.</span></span>

<span data-ttu-id="26d5e-107">Wie können Sie in diesen Fällen, während WSL selbst verfügbar ist, Linux-Distributionen in WSL herunterladen und installieren, wenn Sie nicht auf den Store zugreifen können?</span><span class="sxs-lookup"><span data-stu-id="26d5e-107">In these cases, while WSL itself is available, how do you download and install Linux distros in WSL if you can't access the store?</span></span>

> <span data-ttu-id="26d5e-108">Hinweis: **Befehlszeilenshellumgebungen, einschließlich cmd, PowerShell und Linux/WSL-Distributionen, dürfen im Windows 10 S-Modus nicht ausgeführt werden**.</span><span class="sxs-lookup"><span data-stu-id="26d5e-108">Note: **Command-line shell environments including Cmd, PowerShell, and Linux/WSL distros are not permitted to run on Windows 10 S Mode**.</span></span> <span data-ttu-id="26d5e-109">Diese Einschränkung ist vorhanden, um die Integritäts-und Sicherheitsziele des S-Modus sicherzustellen: Weitere Informationen finden Sie in [diesem Beitrag](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/) .</span><span class="sxs-lookup"><span data-stu-id="26d5e-109">This restriction exists in order to ensure the integrity and safety goals that S Mode delivers: Read [this post](https://blogs.msdn.microsoft.com/commandline/2017/05/18/will-linux-distros-run-on-windows-10-s/) for more information.</span></span>

## <a name="downloading-distros"></a><span data-ttu-id="26d5e-110">Herunterladen von Distributionen</span><span class="sxs-lookup"><span data-stu-id="26d5e-110">Downloading distros</span></span>

<span data-ttu-id="26d5e-111">Wenn die Microsoft Store-App nicht verfügbar ist, können Sie Linux-Distributionen herunterladen und manuell installieren, indem Sie auf die folgenden Links klicken:</span><span class="sxs-lookup"><span data-stu-id="26d5e-111">If the Microsoft Store app is not available, you can download and manually install Linux distros by clicking these links:</span></span>
* [<span data-ttu-id="26d5e-112">Ubuntu 18,04</span><span class="sxs-lookup"><span data-stu-id="26d5e-112">Ubuntu 18.04</span></span>](https://aka.ms/wsl-ubuntu-1804)
* [<span data-ttu-id="26d5e-113">Ubuntu 18,04 Arm</span><span class="sxs-lookup"><span data-stu-id="26d5e-113">Ubuntu 18.04 ARM</span></span>](https://aka.ms/wsl-ubuntu-1804-arm)
* [<span data-ttu-id="26d5e-114">Ubuntu 16.04</span><span class="sxs-lookup"><span data-stu-id="26d5e-114">Ubuntu 16.04</span></span>](https://aka.ms/wsl-ubuntu-1604)
* [<span data-ttu-id="26d5e-115">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="26d5e-115">Debian GNU/Linux</span></span>](https://aka.ms/wsl-debian-gnulinux)
* [<span data-ttu-id="26d5e-116">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="26d5e-116">Kali Linux</span></span>](https://aka.ms/wsl-kali-linux-new)
* [<span data-ttu-id="26d5e-117">OpenSUSE-Schritt 42</span><span class="sxs-lookup"><span data-stu-id="26d5e-117">OpenSUSE Leap 42</span></span>](https://aka.ms/wsl-opensuse-42)
* [<span data-ttu-id="26d5e-118">SUSE Linux Enterprise Server 12</span><span class="sxs-lookup"><span data-stu-id="26d5e-118">SUSE Linux Enterprise Server 12</span></span>](https://aka.ms/wsl-sles-12)
* [<span data-ttu-id="26d5e-119">Fedora Remix für WSL</span><span class="sxs-lookup"><span data-stu-id="26d5e-119">Fedora Remix for WSL</span></span>](https://github.com/WhitewaterFoundry/WSLFedoraRemix/releases/)

<span data-ttu-id="26d5e-120">Dies bewirkt, dass `<distro>.appx` die Pakete in einen Ordner Ihrer Wahl heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="26d5e-120">This will cause the `<distro>.appx` packages to download to a folder of your choosing.</span></span> <span data-ttu-id="26d5e-121">Befolgen Sie die [Installationsanweisungen](#installing-your-distro) , um die heruntergeladenen Distributionen zu installieren.</span><span class="sxs-lookup"><span data-stu-id="26d5e-121">Follow the [installation instructions](#installing-your-distro) to install your downloaded distro(s).</span></span>

## <a name="downloading-distros-via-the-command-line"></a><span data-ttu-id="26d5e-122">Herunterladen von Distributionen über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="26d5e-122">Downloading distros via the command line</span></span>
<span data-ttu-id="26d5e-123">Wenn Sie möchten, können Sie Ihre bevorzugten Distributionen auch über die Befehlszeile herunterladen:</span><span class="sxs-lookup"><span data-stu-id="26d5e-123">If you prefer, you can also download your preferred distro(s) via the command line:</span></span>

 ### <a name="download-using-powershell"></a><span data-ttu-id="26d5e-124">Herunterladen mithilfe von PowerShell</span><span class="sxs-lookup"><span data-stu-id="26d5e-124">Download using PowerShell</span></span>
 <span data-ttu-id="26d5e-125">Verwenden Sie das Cmdlet "Start [-WebRequest](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.utility/invoke-webrequest) ", um Distributionen mithilfe von PowerShell herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="26d5e-125">To download distros using PowerShell, use the [Invoke-WebRequest](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.utility/invoke-webrequest) cmdlet.</span></span> <span data-ttu-id="26d5e-126">Im folgenden finden Sie eine Beispiel Anweisung zum Herunterladen von Ubuntu 16,04.</span><span class="sxs-lookup"><span data-stu-id="26d5e-126">Here's a sample instruction to download Ubuntu 16.04.</span></span>

```powershell
Invoke-WebRequest -Uri https://aka.ms/wsl-ubuntu-1604 -OutFile Ubuntu.appx -UseBasicParsing
```

> [!TIP]
> <span data-ttu-id="26d5e-127">Wenn der Download sehr lange dauert, deaktivieren Sie die Statusanzeige, indem Sie`$ProgressPreference = 'SilentlyContinue'`</span><span class="sxs-lookup"><span data-stu-id="26d5e-127">If the download is taking a long time, turn off the progress bar by setting `$ProgressPreference = 'SilentlyContinue'`</span></span>

### <a name="download-using-curl"></a><span data-ttu-id="26d5e-128">Download mithilfe von curl</span><span class="sxs-lookup"><span data-stu-id="26d5e-128">Download using curl</span></span>
<span data-ttu-id="26d5e-129">Windows 10 Spring 2018 Update (oder höher) umfasst das beliebte [curl-Befehlszeilen Dienstprogramm](https://curl.haxx.se/) , mit dem Sie Webanforderungen (z. b. HTTP Get-, Post-, Put-usw.-Befehle) von der Befehlszeile aus aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="26d5e-129">Windows 10 Spring 2018 Update (or later) includes the popular [curl command-line utility](https://curl.haxx.se/) with which you can invoke web requests (i.e. HTTP GET, POST, PUT, etc. commands) from the command line.</span></span> <span data-ttu-id="26d5e-130">Mit können `curl.exe` Sie die obigen Distributionen herunterladen:</span><span class="sxs-lookup"><span data-stu-id="26d5e-130">You can use `curl.exe` to download the above distros:</span></span>

```console
curl.exe -L -o ubuntu-1604.appx https://aka.ms/wsl-ubuntu-1604
```

<span data-ttu-id="26d5e-131">Im obigen Beispiel `curl.exe` wird ausgeführt (nicht nur `curl`), um sicherzustellen, dass in PowerShell die ausführbare Datei "Real curl" aufgerufen wird, nicht der PowerShell-curl-Alias für " [Aufruf-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6) ".</span><span class="sxs-lookup"><span data-stu-id="26d5e-131">In the above example, `curl.exe` is executed (not just `curl`) to ensure that, in PowerShell, the real curl executable is invoked, not the PowerShell curl alias for [Invoke-WebRequest](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-6)</span></span>

> <span data-ttu-id="26d5e-132">Hinweis: Die `curl` Verwendung von ist möglicherweise vorzuziehen, wenn Sie Download Schritte mithilfe der CMD-Shell und/ `.bat` oder  /  `.cmd` Skripts aufrufen/ausführen müssen.</span><span class="sxs-lookup"><span data-stu-id="26d5e-132">Note: Using `curl` might be preferable if you have to invoke/script download steps using Cmd shell and/or `.bat` / `.cmd` scripts.</span></span>

## <a name="installing-your-distro"></a><span data-ttu-id="26d5e-133">Installieren der Distribution</span><span class="sxs-lookup"><span data-stu-id="26d5e-133">Installing your distro</span></span>
<span data-ttu-id="26d5e-134">Wenn Sie Windows 10 verwenden, können Sie Ihre Distribution mit PowerShell installieren.</span><span class="sxs-lookup"><span data-stu-id="26d5e-134">If you're using Windows 10 you can install your distro with PowerShell.</span></span> <span data-ttu-id="26d5e-135">Navigieren Sie einfach zum Ordner, der die zuvor heruntergeladene Distribution enthält, und führen Sie in diesem Verzeichnis den `app_name` folgenden Befehl aus, wobei der Name der Datei "Distribution. AppX" ist.</span><span class="sxs-lookup"><span data-stu-id="26d5e-135">Simply navigate to folder containing the distro downloaded from above, and in that directory run the following command where `app_name` is the name of your distro .appx file.</span></span>  
```Powershell
Add-AppxPackage .\app_name.appx
```

<span data-ttu-id="26d5e-136">Wenn Sie Windows Server verwenden, finden Sie die Installationsanweisungen auf der [Windows Server](install-on-server.md) -Dokumentationsseite.</span><span class="sxs-lookup"><span data-stu-id="26d5e-136">If you are using Windows server you can find the install instructions on the [Windows Server](install-on-server.md) documentation page.</span></span>

<span data-ttu-id="26d5e-137">Nachdem Ihre Distribution installiert wurde, finden Sie weitere Informationen auf der Seite [intilization Steps (intilization Steps](initialize-distro.md) ), um Ihre neue Distribution zu initialisieren.</span><span class="sxs-lookup"><span data-stu-id="26d5e-137">Once your distro is installed please refer to the [Intilization Steps](initialize-distro.md) page to initialize your new distro.</span></span>
