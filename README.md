# Prediksi Ledakan Alga dengan Varian RNN


## Deskripsi
Proyek ini membangun sistem peringatan dini ledakan alga (algal bloom) dengan memprediksi kenaikan kadar Chlorophyll-a berbasis deret waktu. Saya membandingkan 6 arsitektur Recurrent Neural Network (RNN) dan menemukan bahwa GRU memberikan performa terbaik pada data ini.

## Gambaran Umum
- **Fokus**: peningkatan kadar Klorofil-a untuk peringatan dini algal bloom
- **Model dibandingkan**: RNN, LSTM, GRU, BiRNN, BiLSTM, BiGRU
- **Model terbaik**: GRU
- **Dataset**: `daily_mean.csv` 
  
## Cara Menjalankan 
1. Buka Google Colab 
2. Sediakan data
3. Set path dataset pada notebook sesuai lokasi
4. Instal dependensi
5. Jalankan seluruh sel
