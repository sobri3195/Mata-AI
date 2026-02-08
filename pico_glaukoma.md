# PICO — Mata: AI Skrining Glaukoma Tele-ophthalmology

## Pertanyaan klinis (PICO)
Pada pasien layanan primer/komunitas yang berisiko glaukoma, apakah skrining berbasis AI dari foto fundus smartphone berbiaya rendah yang dikombinasikan dengan faktor risiko klinis, dibandingkan skrining manual (IOP/rujuk berbasis gejala) atau pembacaan fundus oleh dokter umum, dapat meningkatkan akurasi deteksi suspect glaukoma, mengurangi rujukan yang tidak perlu, dan menurunkan keterlambatan diagnosis?

## Komponen PICO
- **P (Population):**
  - Pasien layanan primer/komunitas dengan risiko glaukoma.
  - Contoh faktor risiko: usia >40 tahun, riwayat keluarga glaukoma, miopia tinggi, diabetes/hipertensi, penggunaan steroid jangka panjang.

- **I (Intervention):**
  - Model AI pada foto fundus smartphone low-cost.
  - Input multimodal: citra fundus + variabel riwayat/faktor risiko.
  - Output: rekomendasi **rujuk** vs **lanjut tes/monitor**.

- **C (Comparator):**
  - Skrining manual standar primer care (IOP, gejala, keputusan rujuk rutin).
  - Atau pembacaan foto fundus oleh dokter umum.

- **O (Outcomes):**
  - **Primer:** AUC, sensitivitas (dan spesifisitas) untuk deteksi suspect glaukoma.
  - **Sekunder:**
    - Proporsi rujukan tidak perlu (false-positive referral).
    - Keterlambatan diagnosis (waktu dari skrining ke diagnosis definitif/spesialis).
    - Nilai prediktif positif/negatif, kalibrasi model, dan net benefit (opsional).

## Definisi operasional outcome (disarankan)
- **Suspect glaukoma:** ditetapkan dengan rujukan standar emas (penilaian spesialis + pemeriksaan lapang pandang/OCT/IOP sesuai protokol lokal).
- **Rujukan tidak perlu:** pasien dirujuk tetapi tidak memenuhi kriteria glaukoma/suspect pada evaluasi spesialis.
- **Keterlambatan diagnosis:** jumlah hari dari kunjungan skrining awal ke konfirmasi diagnosis oleh layanan mata sekunder/tersier.

## Hipotesis
1. Model AI multimodal meningkatkan sensitivitas deteksi suspect glaukoma dibanding comparator.
2. Model AI mempertahankan/meningkatkan AUC sekaligus menurunkan rujukan tidak perlu.
3. Triase berbasis AI menurunkan median waktu menuju diagnosis definitif.

## Rekomendasi metrik pelaporan
- ROC-AUC, PR-AUC, sensitivitas, spesifisitas, PPV, NPV (dengan 95% CI).
- Decision-curve analysis untuk menilai utilitas klinis pada berbagai threshold rujuk.
- Subgroup analysis (usia, kualitas foto, komorbid, lokasi layanan).
