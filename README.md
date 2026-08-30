# ANALISIS PERFORMA DETEKSI JENIS KENDARAAN PADA REKAMAN CCTV LALU LINTAS BERDASARKAN KONDISI PENCAHAYAAN

## Deskripsi

Penelitian ini menganalisis performa **YOLOv11** dalam mendeteksi jenis kendaraan pada rekaman CCTV lalu lintas berdasarkan kondisi pencahayaan **daytime** dan **nighttime**.

Data diperoleh dari **Surabaya Intelligent Transportation System (SITS)** dengan empat kelas kendaraan:

- Motorcycle
- Car
- Bus
- Truck

Evaluasi dilakukan melalui tujuh skenario pengujian menggunakan metrik **Precision, Recall, F1-Score, dan mAP50**.

## Hasil Utama

| Skenario | Train | Test | mAP50 |
|---|---|---|---:|
| 1 | Daytime | Daytime | 0.872 |
| 2 | Nighttime | Nighttime | 0.805 |
| 3 | Daytime | Nighttime | 0.568 |
| 4 | Nighttime | Daytime | 0.794 |
| 5 | Combined | Daytime | **0.886** |
| 6 | Combined | Nighttime | 0.809 |
| 7 | Combined | Combined | 0.848 |

**Best Performance:** 0.886 mAP50 — Combined → Daytime

**Lowest Performance:** 0.568 mAP50 — Daytime → Nighttime

## Tools

- Python
- YOLOv11
- OpenCV
- Roboflow
- PyTorch
- Google Colaboratory
