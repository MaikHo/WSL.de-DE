---
title: Installieren des Windows-Subsystems für Linux (WSL) unter Windows 10
description: Installationsanweisungen für das Windows-Subsystem für Linux unter Windows 10.
keywords: BashOnWindows, bash, wsl, windows, windows subsystem for linux, windowssubsystem, ubuntu, debian, suse, windows 10, install
ms.date: 07/23/2018
ms.topic: article
ms.assetid: 7afaeacf-435a-4e58-bff0-a9f0d75b8a51
ms.custom: seodec18
ms.localizationpriority: high
ms.openlocfilehash: 9cd38fbe3781fd0cd45bcd52c278de548d3da38f
ms.sourcegitcommit: 3fb40fd65b34a5eb26b213a0df6a3b2746b7a9b4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/12/2020
ms.locfileid: "83270548"
---
# <a name="install-windows-subsystem-for-linux"></a><span data-ttu-id="82136-104">Installieren des Windows-Subsystems für Linux</span><span class="sxs-lookup"><span data-stu-id="82136-104">Install Windows Subsystem for Linux</span></span>

<span data-ttu-id="82136-105">Im folgenden Leitfaden werden die Schritte beschrieben, die ausgeführt werden müssen, um das Windows-Subsystem für Linux (WSL) auf einem Computer mit Windows 10 zu installieren.</span><span class="sxs-lookup"><span data-stu-id="82136-105">The following guide will walk through the steps required to install the Windows Subsystem for Linux (WSL) on a computer running Windows 10.</span></span>

## <a name="enable-the-windows-subsystem-for-linux-optional-feature"></a><span data-ttu-id="82136-106">Aktivieren des optionalen Features „Windows-Subsystem für Linux“</span><span class="sxs-lookup"><span data-stu-id="82136-106">Enable the Windows Subsystem for Linux optional feature</span></span>

<span data-ttu-id="82136-107">Bevor Sie eine Linux-Verteilung installieren können, müssen Sie das optionale Feature „Windows-Subsystem für Linux“ unter Windows 10 aktivieren:</span><span class="sxs-lookup"><span data-stu-id="82136-107">Before installing a Linux distribution, you must enable the "Windows Subsystem for Linux" optional feature on Windows 10:</span></span>

1. <span data-ttu-id="82136-108">Öffnen Sie PowerShell als Administrator, und geben Sie dieses Skript ein:</span><span class="sxs-lookup"><span data-stu-id="82136-108">Open PowerShell as Administrator and enter this script:</span></span>

```powershell
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

1. <span data-ttu-id="82136-109">Starten Sie den Computer neu, wenn Sie dazu aufgefordert werden.</span><span class="sxs-lookup"><span data-stu-id="82136-109">Restart your computer when prompted.</span></span>

## <a name="install-a-linux-distribution"></a><span data-ttu-id="82136-110">Installieren einer Linux-Distribution</span><span class="sxs-lookup"><span data-stu-id="82136-110">Install a Linux distribution</span></span>

<span data-ttu-id="82136-111">Es gibt drei Möglichkeiten, Ihre bevorzugte(n) Linux-Verteilung(en) herunterzuladen und zu installieren:</span><span class="sxs-lookup"><span data-stu-id="82136-111">There are three ways to download and install your preferred Linux distribution(s):</span></span>

- <span data-ttu-id="82136-112">Herunterladen und Installieren aus dem Microsoft Store (siehe unten)</span><span class="sxs-lookup"><span data-stu-id="82136-112">Download and install from the Microsoft Store (see below)</span></span>
- [<span data-ttu-id="82136-113">Herunterladen und manuelles Installieren über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="82136-113">Download and manually install from command line</span></span>](install-manual.md)
- <span data-ttu-id="82136-114">[Installieren unter Windows Server]]\(install-on-server.md)</span><span class="sxs-lookup"><span data-stu-id="82136-114">[Install on Windows Server]](install-on-server.md)</span></span>

### <a name="install-from-the-microsoft-store"></a><span data-ttu-id="82136-115">Herunterladen aus dem Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="82136-115">Install from the Microsoft Store</span></span>

<span data-ttu-id="82136-116">Linux-Verteilungen können über den Microsoft Store auf Windows 10 (Build 16215+) installiert werden.</span><span class="sxs-lookup"><span data-stu-id="82136-116">Linux distributions can be installed from the Microsoft Store on Windows 10 (Build 16215+).</span></span>

> [!NOTE]
> <span data-ttu-id="82136-117">Führen Sie diese Schritte aus, um [die Nummer Ihres Windows 10-Builds zu überprüfen](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="82136-117">Follow these steps to [check your Windows 10 build number](troubleshooting.md#check-your-build-number).</span></span>

1. <span data-ttu-id="82136-118">Öffnen Sie den Microsoft Store, und wählen Sie Ihre bevorzugte Linux-Distribution aus.</span><span class="sxs-lookup"><span data-stu-id="82136-118">Open the Microsoft Store and choose your favorite Linux distribution.</span></span>

    ![Ansicht der Linux-Distributionen im Microsoft Store](media/store.png)

    <span data-ttu-id="82136-120">Über die folgenden Links wird die Seite des Microsoft Store für jede Distribution geöffnet:</span><span class="sxs-lookup"><span data-stu-id="82136-120">The following links will open the Microsoft store page for each distribution:</span></span>

    - [<span data-ttu-id="82136-121">Ubuntu 16.04 LTS</span><span class="sxs-lookup"><span data-stu-id="82136-121">Ubuntu 16.04 LTS</span></span>](https://www.microsoft.com/store/apps/9pjn388hp8c9)
    - [<span data-ttu-id="82136-122">Ubuntu 18.04 LTS</span><span class="sxs-lookup"><span data-stu-id="82136-122">Ubuntu 18.04 LTS</span></span>](https://www.microsoft.com/store/apps/9N9TNGVNDL3Q)
    - [<span data-ttu-id="82136-123">OpenSUSE Leap 15</span><span class="sxs-lookup"><span data-stu-id="82136-123">OpenSUSE Leap 15</span></span>](https://www.microsoft.com/store/apps/9n1tb6fpvj8c)
    - [<span data-ttu-id="82136-124">OpenSUSE Leap 42</span><span class="sxs-lookup"><span data-stu-id="82136-124">OpenSUSE Leap 42</span></span>](https://www.microsoft.com/store/apps/9njvjts82tjx)
    - [<span data-ttu-id="82136-125">SUSE Linux Enterprise Server 12</span><span class="sxs-lookup"><span data-stu-id="82136-125">SUSE Linux Enterprise Server 12</span></span>](https://www.microsoft.com/store/apps/9p32mwbh6cns)
    - [<span data-ttu-id="82136-126">SUSE Linux Enterprise Server 15</span><span class="sxs-lookup"><span data-stu-id="82136-126">SUSE Linux Enterprise Server 15</span></span>](https://www.microsoft.com/store/apps/9pmw35d7fnlx)
    - [<span data-ttu-id="82136-127">Kali Linux</span><span class="sxs-lookup"><span data-stu-id="82136-127">Kali Linux</span></span>](https://www.microsoft.com/store/apps/9PKR34TNCV07)
    - [<span data-ttu-id="82136-128">Debian GNU/Linux</span><span class="sxs-lookup"><span data-stu-id="82136-128">Debian GNU/Linux</span></span>](https://www.microsoft.com/store/apps/9MSVKQC78PK6)
    - [<span data-ttu-id="82136-129">Fedora Remix for WSL</span><span class="sxs-lookup"><span data-stu-id="82136-129">Fedora Remix for WSL</span></span>](https://www.microsoft.com/store/apps/9n6gdm4k2hnc)
    - [<span data-ttu-id="82136-130">Pengwin</span><span class="sxs-lookup"><span data-stu-id="82136-130">Pengwin</span></span>](https://www.microsoft.com/store/apps/9NV1GV1PXZ6P)
    - [<span data-ttu-id="82136-131">Pengwin Enterprise</span><span class="sxs-lookup"><span data-stu-id="82136-131">Pengwin Enterprise</span></span>](https://www.microsoft.com/store/apps/9N8LP0X93VCP)
    - [<span data-ttu-id="82136-132">Alpine WSL</span><span class="sxs-lookup"><span data-stu-id="82136-132">Alpine WSL</span></span>](https://www.microsoft.com/store/apps/9p804crf0395)

1. <span data-ttu-id="82136-133">Wählen Sie „Get“ aus, und klicken Sie nach dem Herunterladen der Verteilung auf „Starten“.</span><span class="sxs-lookup"><span data-stu-id="82136-133">Select "Get" and once the distribution has finished downloading, select "Launch".</span></span>

    ![Ansicht der Linux-Distributionen im Microsoft Store](media/UbuntuStore.png)

## <a name="complete-initialization-of-your-distro"></a><span data-ttu-id="82136-135">Vervollständigen der Initialisierung Ihrer Distribution</span><span class="sxs-lookup"><span data-stu-id="82136-135">Complete initialization of your distro</span></span>

<span data-ttu-id="82136-136">Nachdem Sie Ihre Linux-Verteilung gestartet haben, befolgen Sie die Anweisungen auf dem Bildschirm, um Ihre Verteilung zu initialisieren.</span><span class="sxs-lookup"><span data-stu-id="82136-136">After launching your Linux distribution, follow the onscreen instructions to initialize your distro.</span></span>

> [!NOTE]
> <span data-ttu-id="82136-137">Starten Sie die Verteilung für Windows Server mithilfe der ausführbaren Datei `<distro>.exe` im Installationsordner.</span><span class="sxs-lookup"><span data-stu-id="82136-137">For Windows Server, launch your distribution using the executable, `<distro>.exe`, in the installation folder.</span></span>

<span data-ttu-id="82136-138">Wenn eine neu installierte Verteilung zum ersten Mal ausgeführt wird, wird ein Konsolenfenster geöffnet, und Sie werden aufgefordert, bis zum Abschluss der Installation wenige Minuten zu warten.</span><span class="sxs-lookup"><span data-stu-id="82136-138">The first time a newly installed distribution runs, a console window will open and you'll be asked to wait for a minute or two for the installation to complete.</span></span> <span data-ttu-id="82136-139">In dieser letzten Phase der Installation werden die Dateien der Distribution dekomprimiert und auf Ihrem PC gespeichert. Sie sind dann einsatzbereit.</span><span class="sxs-lookup"><span data-stu-id="82136-139">During this final stage of installation, the distro's files are de-compressed and stored on your PC, ready for use.</span></span> <span data-ttu-id="82136-140">Dies kann je nach Leistung der Speichergeräte Ihres PCs etwa eine Minute oder ggf. auch länger dauern.</span><span class="sxs-lookup"><span data-stu-id="82136-140">This may take around a minute or more depending on the performance of your PC's storage devices.</span></span> <span data-ttu-id="82136-141">Diese erste Installationsphase ist nur erforderlich, wenn eine „saubere“ Distribution installiert wird. Alle zukünftigen Starts sollten weniger als eine Sekunde in Anspruch nehmen.</span><span class="sxs-lookup"><span data-stu-id="82136-141">This initial installation phase is only required when a distro is clean-installed - all future launches should take less than a second.</span></span>

## <a name="set-up-a-new-linux-user-account"></a><span data-ttu-id="82136-142">Einrichten eines neuen Linux-Benutzerkontos</span><span class="sxs-lookup"><span data-stu-id="82136-142">Set up a new Linux user account</span></span>

<span data-ttu-id="82136-143">Nach Abschluss der Installation werden Sie aufgefordert, ein neues Benutzerkonto (und das zugehörige Kennwort) zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="82136-143">Once installation is complete, you will be prompted to create a new user account (and its password).</span></span>

![Entpacken von Ubuntu in der Windows-Konsole](media/UbuntuInstall.png)

<span data-ttu-id="82136-145">Dieses Benutzerkonto gilt für den normalen Benutzer ohne Administratorrechte, als der Sie beim Starten einer Verteilung standardmäßig angemeldet werden.</span><span class="sxs-lookup"><span data-stu-id="82136-145">This user account is for the normal non-admin user that you'll be logged-in as by default when launching a distribution.</span></span> <span data-ttu-id="82136-146">Sie können einen beliebigen Benutzernamen und ein gewünschtes Kennwort auswählen. Beides hat keinen Einfluss auf Ihren Windows-Benutzernamen.</span><span class="sxs-lookup"><span data-stu-id="82136-146">You can choose any username and password you wish - they have no bearing on your Windows username.</span></span>

<span data-ttu-id="82136-147">Wenn Sie eine neue Distributionsinstanz öffnen, werden Sie nicht zur Eingabe Ihres Kennworts aufgefordert. Wenn Sie jedoch **einen Prozess mit `sudo` heraufstufen, müssen Sie Ihr Kennwort eingeben**. Stellen Sie also sicher, dass Sie ein Kennwort auswählen, das Sie sich leicht merken können.</span><span class="sxs-lookup"><span data-stu-id="82136-147">When you open a new distro instance, you won't be prompted for your password, but **if you elevate a process using `sudo`, you will need to enter your password**, so make sure you choose a password you can easily remember!</span></span> <span data-ttu-id="82136-148">Weitere Informationen finden Sie auf der Seite [Benutzersupport](user-support.md).</span><span class="sxs-lookup"><span data-stu-id="82136-148">See the [User Support](user-support.md) page for more info.</span></span>

## <a name="update--upgrade-packages"></a><span data-ttu-id="82136-149">Update- und Upgradepakete</span><span class="sxs-lookup"><span data-stu-id="82136-149">Update & upgrade packages</span></span>

<span data-ttu-id="82136-150">Die meisten Verteilungen werden mit einem leeren oder minimalen Paketkatalog ausgeliefert.</span><span class="sxs-lookup"><span data-stu-id="82136-150">Most distributions ship with an empty or minimal package catalog.</span></span> <span data-ttu-id="82136-151">Es wird dringend empfohlen, den Paketkatalog regelmäßig zu aktualisieren und ein Upgrade der installierten Pakete mit dem bevorzugten Paket-Manager Ihrer Verteilung auszuführen.</span><span class="sxs-lookup"><span data-stu-id="82136-151">We strongly recommend regularly updating your package catalog and upgrading your installed packages using your distro's preferred package manager.</span></span> <span data-ttu-id="82136-152">Für Debian/Ubuntu verwenden Sie apt:</span><span class="sxs-lookup"><span data-stu-id="82136-152">For Debian/Ubuntu, use apt:</span></span>

```bash
sudo apt update && sudo apt upgrade
```

<span data-ttu-id="82136-153">Windows führt für Ihre Linux-Verteilung(en) nicht automatisch eine Aktualisierung oder ein Upgrade aus.</span><span class="sxs-lookup"><span data-stu-id="82136-153">Windows does not automatically update or upgrade your Linux distro(s).</span></span> <span data-ttu-id="82136-154">Dies ist eine Aufgabe, die die meisten Linux-Benutzer lieber selbst in die Hand nehmen.</span><span class="sxs-lookup"><span data-stu-id="82136-154">This is a task that the most Linux users prefer to control themselves.</span></span>

<span data-ttu-id="82136-155">Viel Spaß bei der Verwendung Ihrer neuen Linux-Distribution unter WSL!</span><span class="sxs-lookup"><span data-stu-id="82136-155">Enjoy using your new Linux distro on WSL!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="82136-156">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="82136-156">Troubleshooting</span></span>

<span data-ttu-id="82136-157">Nachfolgend werden einige Installationsfehler und vorgeschlagene Korrekturen beschrieben.</span><span class="sxs-lookup"><span data-stu-id="82136-157">Below are related installation errors and suggested fixes.</span></span> <span data-ttu-id="82136-158">Weitere allgemeine Fehler und zugehörige Lösungen finden Sie auf der [Seite für die WSL-Problembehandlung](troubleshooting.md).</span><span class="sxs-lookup"><span data-stu-id="82136-158">Refer to the [WSL troubleshooting page](troubleshooting.md) for other common errors and their solutions.</span></span>

### <a name="installation-failed-with-error-0x8007007e"></a><span data-ttu-id="82136-159">Installationsfehler mit Fehlercode 0x8007007e</span><span class="sxs-lookup"><span data-stu-id="82136-159">Installation failed with error 0x8007007e</span></span>

<span data-ttu-id="82136-160">Dieser Fehler tritt auf, wenn das System Linux aus dem Store nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82136-160">This error occurs when your system doesn't support Linux from the store.</span></span>  <span data-ttu-id="82136-161">Stellen Sie Folgendes sicher:</span><span class="sxs-lookup"><span data-stu-id="82136-161">Make sure that:</span></span>

- <span data-ttu-id="82136-162">Sie führen Windows-Build 16215 oder höher aus.</span><span class="sxs-lookup"><span data-stu-id="82136-162">You're running Windows build 16215 or later.</span></span> <span data-ttu-id="82136-163">[Überprüfen Sie Ihren Build](troubleshooting.md#check-your-build-number).</span><span class="sxs-lookup"><span data-stu-id="82136-163">[Check your build](troubleshooting.md#check-your-build-number).</span></span>
- <span data-ttu-id="82136-164">Die optionale Komponente des Windows-Subsystems für Linux ist aktiviert, und der Computer wurde neu gestartet.</span><span class="sxs-lookup"><span data-stu-id="82136-164">The Windows Subsystem for Linux optional component is enabled and the computer has restarted.</span></span>  <span data-ttu-id="82136-165">[Stellen Sie sicher, dass WSL aktiviert ist](troubleshooting.md#confirm-wsl-is-enabled).</span><span class="sxs-lookup"><span data-stu-id="82136-165">[Make sure WSL is enabled](troubleshooting.md#confirm-wsl-is-enabled).</span></span>

### <a name="installation-failed-with-error-0x80070003"></a><span data-ttu-id="82136-166">Installationsfehler mit Fehlercode 0x80070003</span><span class="sxs-lookup"><span data-stu-id="82136-166">Installation failed with error 0x80070003</span></span>

<span data-ttu-id="82136-167">Das Windows-Subsystem für Linux wird nur auf dem Systemlaufwerk ausgeführt (in der Regel ist dies Ihr Laufwerk `C:`).</span><span class="sxs-lookup"><span data-stu-id="82136-167">The Windows Subsystem for Linux only runs on your system drive (usually this is your `C:` drive).</span></span> <span data-ttu-id="82136-168">Stellen Sie sicher, dass die Distributionen auf dem Systemlaufwerk gespeichert sind:</span><span class="sxs-lookup"><span data-stu-id="82136-168">Make sure that distros are stored on your system drive:</span></span>

- <span data-ttu-id="82136-169">Öffnen Sie **Einstellungen** -> **Speicher** -> **Weitere Speichereinstellungen: Ändern Sie den Speicherort für neue Inhalte**</span><span class="sxs-lookup"><span data-stu-id="82136-169">Open **Settings** -> **Storage** -> **More Storage Settings: Change where new content is saved**</span></span>
  
    ![Abbildung der Systemeinstellungen für die Installation von Apps auf dem Laufwerk C:](media/AppStorage.png)

### <a name="wslregisterdistribution-failed-with-error-0x8007019e"></a><span data-ttu-id="82136-171">WslRegisterDistribution-Fehler mit Fehlercode 0x8007019e</span><span class="sxs-lookup"><span data-stu-id="82136-171">WslRegisterDistribution failed with error 0x8007019e</span></span>

<span data-ttu-id="82136-172">Die optionale Komponente des Windows-Subsystems für Linux ist nicht aktiviert:</span><span class="sxs-lookup"><span data-stu-id="82136-172">The Windows Subsystem for Linux optional component is not enabled:</span></span>

- <span data-ttu-id="82136-173">Öffnen Sie **Systemsteuerung** -> **Programme und Funktionen** -> **Windows-Funktion aktivieren oder deaktivieren**. Aktivieren Sie die Option **Windows-Subsystem für Linux**, oder verwenden Sie das PowerShell-Cmdlet, das am Anfang dieses Artikels erwähnt wurde.</span><span class="sxs-lookup"><span data-stu-id="82136-173">Open **Control Panel** -> **Programs and Features** -> **Turn Windows Feature on or off** -> Check **Windows Subsystem for Linux** or using the PowerShell cmdlet mentioned at the begining of this article.</span></span>
