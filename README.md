# Algal Bloom Forecasting with RNN Variants

Proyek ini membangun sistem peringatan dini ledakan alga (algal bloom) dengan memprediksi kenaikan kadar Chlorophyll-a berbasis deret waktu. Kami membandingkan 6 arsitektur Recurrent Neural Network (RNN) dan menemukan bahwa GRU memberikan performa terbaik pada data ini.

## Ringkasan
- **Fokus**: Forecasting Chlorophyll-a untuk peringatan dini algal bloom
- **Model dibandingkan**: RNN, LSTM, GRU, BiRNN, BiLSTM, BiGRU
- **Model terbaik**: GRU
- **Dataset**: `daily_mean.csv` (time series harian)

## Struktur Repo
```
├── Final_Source_Code_RNN_Ahmad Dzaki Alfarouq.ipynb
├── Final_Source_Code_LSTM_Ahmad Dzaki Alfarouq.ipynb
├── Final_Source_Code_GRU_Ahmad Dzaki Alfarouq.ipynb
├── Final_Source_Code_BiRNN_Ahmad Dzaki Alfarouq.ipynb
├── Final_Source_Code_BiLSTM_Ahmad Dzaki Alfarouq.ipynb
├── Final_Source_Code_BiGRU_Ahmad Dzaki Alfarouq.ipynb
├── daily_mean.csv
├── .gitignore
└── README.md
```

## Persiapan Lingkungan
Disarankan Python 3.9+ dan virtual environment.

```bash
# (opsional) buat env
python -m venv .venv

# aktifkan (Windows PowerShell)
. .venv/Scripts/Activate.ps1

# update pip
python -m pip install --upgrade pip
```

Install dependensi umum:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
pip install tensorflow==2.*  # atau torch jika notebook pakai PyTorch
```

## Cara Menjalankan
1. Buka Jupyter:
   ```bash
   jupyter notebook
   ```
2. Buka salah satu notebook model (mis. `Final_Source_Code_GRU_...ipynb`).
3. Pastikan path dataset `daily_mean.csv` sesuai.
4. Jalankan seluruh sel (Kernel → Restart & Run All).

## Data
- **Berkas**: `daily_mean.csv`
- **Frekuensi**: Harian
- **Target**: Chlorophyll-a
- Pastikan preprocessing di setiap notebook sesuai dengan skema kolom pada dataset.

## Hasil
Ringkas hasil utama (silakan ganti dengan angka aktual dari eksperimen Anda):
- **GRU**: MAE = ..., RMSE = ..., MAPE = ... (Model Terbaik)
- **LSTM**: MAE = ..., RMSE = ..., MAPE = ...
- **RNN**: MAE = ..., RMSE = ..., MAPE = ...
- **BiLSTM**: MAE = ..., RMSE = ..., MAPE = ...
- **BiGRU**: MAE = ..., RMSE = ..., MAPE = ...
- **BiRNN**: MAE = ..., RMSE = ..., MAPE = ...

**Kesimpulan**: GRU konsisten unggul pada metrik utama dan stabilitas training.

## Reproduksibilitas
- Set random seed di setiap notebook (jika ada).
- Laporkan konfigurasi: window size, horizon, normalisasi, train/val/test split.

## Kontributor
- **Ahmad Dzaki Alfarouq** - Penulis utama

## Lisensi
MIT License - silakan gunakan untuk keperluan akademik dan penelitian.

---
*Repository ini berisi implementasi perbandingan 6 varian RNN untuk prediksi Chlorophyll-a dalam konteks peringatan dini algal bloom.*
