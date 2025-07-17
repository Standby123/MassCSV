# MassCSV

**MassCSV** is a desktop application for exploring, filtering, and analyzing large CSV and Parquet datasets — with advanced time-series and signal processing tools built in.

Designed for engineers, scientists, and analysts, MassCSV offers real-time plotting, interactive filtering, FFT analysis, and export functionality in a simple, fast GUI.

---

## 🧰 Features

- 📁 **Load Large Datasets**: Supports CSV and Parquet files with custom delimiters
- 🕒 **Time-Aware X-Axis**: Use raw time values or convert to datetimes
- 📊 **Multiple Y-Series Plotting**
- ⚙️ **Interactive Filters**:
  - Scale Y data
  - Set upper/lower thresholds
  - Remove mid-band noise
- 🖱️ **Cursor Tool**: View exact values on hover with optional annotations
- 📈 **FFT Viewer**: Frequency spectrum with log scaling & peak detection
- 📋 **Statistics Tab**: Mean, variance, and interval analysis
- 💾 **Export Filtered Data** to new CSV files
- 🌓 **Dark mode support** (coming soon!)

---

## 🚀 Getting Started

### 1. Run the App

If you received `MassCSV.exe`, just double-click to launch.

> No installation required. No Python needed.

If you see a SmartScreen warning, click **"More info → Run anyway"** (Windows shows this for unsigned apps).

---

### 2. Load Data

- Click **"Browse"** to select a `.csv` or `.parquet` file
- Choose your **X-axis** column (e.g. time)
- Select one or more **Y-axis** columns
- Click **"Plot"**

---

### 3. Apply Filters

- Use the **Y-min** / **Y-max** inputs to remove outliers or noise
- Use the **Y-scale** box to apply gain/multipliers
- Click **"Export"** to save the filtered view to a new CSV

---

### 4. Analyze

- Use the **Statistics tab** to view detailed metrics
- Use the **FFT tab** to analyze frequency content
  - Toggle **Log X/Y** scales
  - Hover to view peak frequency markers

---

## 💾 Export Options

- Filtered plots can be exported as `.png` or `.csv`
- Filter settings are respected when exporting

---

## ❓ FAQ

**Q: Do I need to install anything?**  
A: No. MassCSV is a standalone `.exe` file that runs on Windows 10/11.

**Q: Does it work with huge files?**  
A: Yes — it processes data in batches and downscales automatically for speed.

**Q: Can I edit the code?**  
A: Yes — the app is written in Python (PyQt5 + Matplotlib + Polars). If you want to run or modify the source code, install the dependencies listed below.

---

## 🧪 Developer Mode (Optional)

If you'd like to run from source:

```bash
git clone https://github.com/Standby123/MassCSV.git
cd MassCSV
pip install -r requirements.txt
python Application.py
```

### Dependencies:
- `PyQt5`
- `matplotlib`
- `pandas`
- `polars`
- `scipy`
- `numpy`

---

## 📦 Build as .EXE (Advanced)

Use `PyInstaller`:

```bash
pyinstaller --onefile --windowed --noconsole --icon=icon.ico Application.py
```

---

## 📣 License

This project is shared for free under the MIT License.  
Use it, modify it, and share it — just give credit.

---

## ✉️ Contact

**Author**: Sean Feely  
**Email**: [Feelysean15@gmail.com](mailto:Feelysean15@gmail.com)  
**GitHub**: [https://github.com/Standby123/MassCSV/tree/main](https://github.com/Standby123/MassCSV/tree/main)

---

**Enjoy exploring your data at scale with MassCSV!**
