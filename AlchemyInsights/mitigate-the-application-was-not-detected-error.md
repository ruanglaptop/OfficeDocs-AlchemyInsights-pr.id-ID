---
title: Mitigasi kesalahan Aplikasi tidak terdeteksi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810487"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="74c36-102">Mitigasi kesalahan "Aplikasi tidak terdeteksi"</span><span class="sxs-lookup"><span data-stu-id="74c36-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="74c36-103">Kesalahan penginstalan aplikasi, “Aplikasi tidak terdeteksi setelah penginstalan berhasil diselesaikan,” dilaporkan oleh Intune, mungkin terjadi di semua platform OS utama (Windows, iOS, dan Android).</span><span class="sxs-lookup"><span data-stu-id="74c36-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="74c36-104">Skenario paling umum yang menghasilkan kesalahan ini mencakup:</span><span class="sxs-lookup"><span data-stu-id="74c36-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="74c36-105">Aplikasi telah diperbarui di luar Intune (dari bursa aplikasi pihak ketiga) setelah penyebaran awal.</span><span class="sxs-lookup"><span data-stu-id="74c36-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="74c36-106">Misalnya, beberapa aplikasi seperti Google Chrome mungkin menjalankan pembaruan otomatis.</span><span class="sxs-lookup"><span data-stu-id="74c36-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="74c36-107">Pengguna telah menghapus instalan aplikasi setelah penginstalan awal.</span><span class="sxs-lookup"><span data-stu-id="74c36-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="74c36-108">Untuk memitigasi masalah ini, lakukan peninjauan terlebih dahulu terhadap perangkat yang terpengaruh guna menentukan skenario terjadinya kesalahan.</span><span class="sxs-lookup"><span data-stu-id="74c36-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="74c36-109">Jika aplikasi telah diperbarui di luar Intune, penyebaran aplikasi dapat diatur untuk mengabaikan versi aplikasi.</span><span class="sxs-lookup"><span data-stu-id="74c36-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="74c36-110">Untuk melakukannya, di bawah **Konfigurasi Aplikasi > Informasi Aplikasi**, atur **Abaikan Versi Aplikasi** ke **Ya**.</span><span class="sxs-lookup"><span data-stu-id="74c36-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="74c36-111">Saat menargetkan klien, mungkin tepat untuk menyebarkan aplikasi sebagai “diperlukan,” dan untuk memastikan bahwa versi terbaru disebarkan.</span><span class="sxs-lookup"><span data-stu-id="74c36-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="74c36-112">Alternatifnya, di platform iOS, dimungkinkan untuk menggunakan fungsi **autoupdate** yang terkait dengan Program Pembelian Volume Apple, yang dapat dikonfigurasi agar secara otomatis memperbarui ke versi aplikasi baru saat tersedia.</span><span class="sxs-lookup"><span data-stu-id="74c36-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="74c36-113">Untuk informasi selengkapnya tentang pemecahan masalah penginstalan aplikasi, silakan lihat [Memecahkan masalah penginstalan aplikasi](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="74c36-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>