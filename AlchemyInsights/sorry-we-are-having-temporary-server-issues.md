---
title: Memperbaiki aplikasi Office Maaf, kami mengalami pesan masalah server sementara
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627993"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Memperbaiki aplikasi Office "Maaf, kami mengalami masalah server sementara" pesan

Jika Anda menerima pesan ini, cobalah berikut ini:

1. Periksa firewall, perangkat lunak antivirus, dan pengaturan proxy untuk mengonfirmasi bahwa mereka tidak memblokir akses internet ke aplikasi Office. Lihat [Office 365 URL dan kisaran alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Pergi ke **mulai** > **menjalankan**, dan kemudian ketik **Services. MSC**. Pastikan bahwa layanan berikut ini berjalan:
    - Jaringan tersambung perangkat Auto-setup
    - Layanan daftar jaringan
    - Kesadaran lokasi jaringan
    - Log peristiwa Windows

Jika salah satu layanan ini tidak berjalan, cobalah untuk memulainya. Jika Anda memiliki masalah memulai layanan, jalankan perintah berikut ini dengan membuka prompt perintah dengan izin yang ditinggikan:

**SFC/SCANNOW**

Setelah perintah ini selesai, mulai ulang komputer.

Untuk informasi terperinci, lihat ["Maaf, kami tidak dapat tersambung ke akun Anda. Silakan coba lagi nanti "galat saat Anda mengaktifkan Office dari Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).