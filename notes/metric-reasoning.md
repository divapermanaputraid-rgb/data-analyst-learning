# Metric Reasoning Log

File ini berisi catatan cara saya memahami dan membingkai metric
selama proses belajar data analytics.

Fokus utama:
- membedakan aktivitas vs value
- memahami hierarki metric
- menghindari interpretasi yang menyesatkan


## Aktivitas ≠ Value

Metric seperti:
- session
- watch hour
- transaction count

adalah **metric aktivitas**.

Metric ini hanya menunjukkan bahwa user melakukan sesuatu,
bukan bahwa bisnis mendapatkan nilai.

Aktivitas baru bernilai jika:
monetisasi yang dihasilkan ≥ biaya yang ditimbulkan.

Kesalahan umum yang saya sadari:
menganggap kenaikan aktivitas otomatis berarti kondisi bisnis membaik.


## Metric Harus Menyentuh Uang

Pertanyaan bisnis paling dasar:
“Apakah bisnis ini sehat?”

Pertanyaan ini **tidak bisa dijawab** dengan:
- DAU
- watch hour
- total session

Metric utama harus menyentuh uang, seperti:
- net revenue per user
- revenue per hour
- contribution margin (jika data tersedia)

Tanpa itu, grafik pertumbuhan hanya menunjukkan kesibukan,
bukan keberlanjutan.


## Hierarki Metric (yang sering bocor)

Urutan yang benar:
1. Primary metric (outcome bisnis)
2. Supporting metrics (penjelas)
3. Guardrail metrics (pencegah salah tafsir)

Kesalahan yang sering terjadi:
- supporting metric diperlakukan seperti primary
- guardrail diabaikan saat grafik terlihat “bagus”

Contoh:
Watch hour naik terlihat positif,
padahal cost per hour naik lebih cepat dari ad revenue per hour.


## Activity Metric sebagai Input, Bukan Outcome

Watch hour, session, repeat active days:
- bukan tujuan akhir
- tapi input ke sistem monetisasi dan biaya

Kesalahan berpikir:
“Meningkatkan watch hour = meningkatkan value”

Pendekatan yang lebih aman:
“Meningkatkan watch hour **perlu divalidasi**
dengan monetisasi dan cost.”


## Catatan Pembelajaran Sementara

Metric yang bagus:
- membantu menjawab pertanyaan bisnis
- mencegah optimisme palsu
- memaksa melihat trade-off

Metric yang berbahaya:
- terlihat intuitif
- mudah naik
- tapi tidak terhubung langsung ke profitabilitas


File ini akan terus diperbarui seiring bertambahnya case study
dan kesalahan berpikir yang saya temui.
