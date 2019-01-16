---
title: Memecahkan masalah dengan mendaftarkan perangkat Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295392"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Memecahkan masalah dengan mendaftarkan perangkat Windows Microsoft Intune

Tinjau sumber daya berikut untuk menyelesaikan masalah Anda sekarang. 
  
Beberapa pesan kesalahan umum dan langkah-langkah resolusi:
  
 **Perangkat lunak tidak dapat diinstal, 0x80cf4017:** Sertifikat akun Anda telah kedaluwarsa. Download ulang paket perangkat lunak PC Client di Konsol Admin Intune. Meninjau dokumentasi ini untuk informasi lebih lanjut. 
  
 **Kode kesalahan 0x801c0003:** Kesalahan dapat terjadi dalam skenario berikut: 
  
1. Pengguna memiliki lebih perangkat yang terdaftar dari batas perangkat. Meninjau dokumen-dokumen ini untuk [menghapus perangkat](https://docs.microsoft.com/en-us/intune/devices-wipe) atau [mengubah batas perangkat](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Pengguna dapat bergabung perangkat Azure iklan" diatur ke "tidak". Set ke semua atau pilih pengguna. Meninjau [dokumentasi ini](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) untuk informasi lebih lanjut. 
    
3. Perangkat sudah terdaftar oleh pengguna lain. Jika itu adalah kasus, menghapus perangkat dari konsol Azure Intune atau secara manual unenroll perangkat sebelum mencoba lagi.
    
4. Perangkat ini Windows 10 Home. Hanya Windows 10 Pro, pendidikan dan Enterprise SKU dapat bergabung Azure Active Directory.
    
Sumber daya tambahan untuk membantu menyelesaikan masalah Anda:
  
1. Gunakan [Intune pemecahan masalah Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) untuk mendiagnosa dan mengatasi gangguan pendaftaran umum. Meninjau [dokumen ini](https://docs.microsoft.com/en-us/intune/help-desk-operators) untuk rincian lebih lanjut. 
    
2. Meninjau dokumen-dokumen ini untuk daftar kesalahan umum yang mencegah pendaftaran dan resolusi untuk masing-masing: [panduan mengatasi masalah](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) dan [mengatasi masalah doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Belajar bagaimana untuk mendaftar perangkat Windows Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).
  
