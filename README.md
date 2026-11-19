# Proyek Analisis Data — Bike Sharing Dataset

Proyek ini dikembangkan dari notebook analisis Bike Sharing Dataset. Isinya meliputi 2 pertanyaan bisnis SMART, data wrangling, EDA, visualisasi, kesimpulan/rekomendasi, teknik binning sederhana, dan dashboard Streamlit.

## Struktur folder

```text
Proyek_Analisis_Data_Bike Sharing_Dicoding/
├── dashboard/
│   ├── dashboard.py
│   ├── main_data.csv
│   └── day_data.csv
├── data/
│   ├── day.csv
│   ├── hour.csv
│   └── Readme.txt
├── notebook.ipynb
├── README.md
├── requirements.txt
└── url.txt
```

## Cara menjalankan dashboard di laptop

1. Ekstrak ZIP lalu buka terminal/PowerShell pada folder utama yang berisi `requirements.txt`.
2. Pastikan Python sudah tersedia (`python --version`).
3. Instal dependensi:

   ```powershell
   python -m pip install -r requirements.txt
   ```

4. Jalankan dashboard:

   ```powershell
   python -m streamlit run dashboard/dashboard.py
   ```

5. Browser biasanya membuka `http://localhost:8501` secara otomatis.

Gunakan filter tanggal dan jenis hari pada sidebar untuk membandingkan pola penyewaan.

## Cara menjalankan notebook

### Di Google Colab

1. Buka `notebook.ipynb` dengan Google Colab.
2. Upload `day.csv` dan `hour.csv` ke panel **Files** sehingga berada di `/content/`.
3. Pilih **Runtime > Run all**. Sel *Gathering Data* otomatis membaca data dari `/content/` jika folder `data/` tidak tersedia.
4. Jika menjalankan sel ekspor di Colab, file dashboard CSV baru berada di `/content/dashboard/`; unduh jika ingin memindahkannya ke laptop. Dalam ZIP ini, file ekspor sudah disertakan.

### Di laptop (Jupyter/VS Code)

1. Buka `notebook.ipynb` dari folder proyek.
2. Pastikan terminal/notebook menggunakan **working directory** folder utama proyek.
3. Jalankan semua sel secara berurutan. File dataset berada pada `data/`.

## Pertanyaan bisnis

1. Bagaimana perbedaan rata-rata penyewaan sepeda per jam antara hari kerja dan nonkerja pada 2011–2012, serta jam mana yang menjadi waktu tersibuk?
2. Bagaimana perbedaan rata-rata penyewaan sepeda harian berdasarkan musim dan kondisi cuaca sepanjang 2011–2012?

## Catatan

- Rata-rata per jam dan rata-rata per hari menggunakan unit analisis yang berbeda.
- Grafik menunjukkan asosiasi/perbedaan deskriptif, bukan bukti sebab-akibat.
- Dashboard telah di-deploy dan alamatnya tercantum di `url.txt`: https://nathania-bike-sharing-dicoding.streamlit.app/
- ID Dicoding pada notebook wajib cocok dengan Username pada Pengaturan akun Dicoding pemilik submission.
