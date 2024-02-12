berikut model Automatic Speech Recognition
Penjelasan Model:
Automatic Speech Recognition (ASR) mengonversi sinyal suara menjadi teks, memetakan sequence input audio ke output teks,seperti halnya dalam teknologi Asisten Virtual "Hello Google"dan "Siri"


tujuan model kali ini adalah:
1. Meningkatkan pemahaman materi dan praktek Tugas NLP pengenalan Suara
2. Menyelesaikan masalah Pengenalan Ucapan/Suara, agar model dapat memahami audio dengan ragam pola bicara, gaya bahasa, gaya bicara, dialek dan frasa yang berbeda.

Langkah pengerjaan:
1. Perbanyak membaca paper  dan percobaan model task voice Recognition
2. tentukan objektif
3. load data set
4. pre-process data sesuai kebutuhan modelnya
   cek transkipsi data, remove punctuation, ubah sampling rate audio sesuai pre-trained modelyg akan kita pakai (whisper)
5. Exploratory Data Analyst, perhatikan juga struktur data, keseimbangan data antar bahasa dan frekuensi suaranya
6. gali lebih dalam fitur dalam suara yg di test dengan extract dataset memakai feature extractor
7. Split data menjadi Train : test (80%:20%)
8. Persiapkan model,dengan define data collator yg dipakai (seq2seq with padding)
9. tentukan metrix evaluasi yg digunakan(Wer)
10. training model
11. predict dan evaluate model

Source dataset ASR:
https://huggingface.co/datasets/timit_asr
https://huggingface.co/datasets/PolyAI/minds14
