---
title: Simulator serangan 2681 di Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801554"
---
# <a name="attack-simulator-in-microsoft-365"></a>Serangan Simulator di Microsoft 365

- Apakah Anda kehilangan serangan Simulator? Simulator serangan memerlukan **Microsoft Defender untuk office 365 paket 2 (paket ATP 2)** atau **Office 365 Enterprise E5** . Simulator serangan **tidak** disertakan dalam Microsoft Defender untuk Office 365 paket 1 (paket ATP 1), Office 365 Enterprise E3, atau aplikasi Microsoft 365 untuk langganan bisnis.

- Akun yang Anda gunakan untuk meluncurkan serangan simulasi memerlukan izin administrator global atau administrator keamanan dan multi-Factor Authentication (MFA). Untuk informasi selengkapnya tentang persyaratan serangan Simulator, lihat [topik ini](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Hal penting yang perlu diketahui tentang simulasi serangan **kata sandi Brute Force** :

  - Jika akun target telah diaktifkan MFA dan kata sandinya sudah benar, akun tidak akan terlihat seperti dikompromikan (faktor autentikasi kedua tidak akan selesai).

  - File kata sandi tidak boleh lebih besar dari 10 MB. Gunakan satu kata sandi per baris, dan sertakan baris kosong (carriage return) setelah kata sandi terakhir dalam daftar.

- Hal penting yang perlu diketahui tentang simulasi lampirkan **Pengelabuan** :

  - Dengan desain, Anda tidak dapat memberikan nilai kustom untuk **URL server login Pengelabuan** .

  - Jika Penerima menggunakan [Add-in Aktifkan pesan laporan](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) untuk melaporkan pesan sebagai Pengelabuan, Anda mungkin tidak menerima pemberitahuan untuk pesan (karena ini adalah serangan simulasi).

- Laporan: setelah serangan simulasi selesai, Anda bisa mengklik **detail serangan** untuk melihat laporan.

- Untuk instruksi mendetail dan fitur baru dalam simulator serangan, lihat [Attack Simulator di Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
