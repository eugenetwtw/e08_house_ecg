# House ECG - Structural Health Monitoring Concept

## 房屋心電圖 - 結構健康監測概念 張渝江土木技師 美國AI工程鑑定學會理事長

### Overview / 概述

**English:**  
House ECG is a conceptual simulation of an app designed to repurpose outdated iPhones as tools for monitoring the structural stiffness of buildings or bridges. By attaching an iPhone to a wall and keeping it powered, the app records acceleration data during earthquakes. This data is synchronized with meteorological station data, transformed into the frequency domain using Fourier Transform, and stored in a database. Each earthquake's frequency domain information is compared with previous records to detect changes in structural stiffness. If a significant change is detected, indicating potential structural damage, the system emails the user to recommend a professional inspection.

**中文:**  
房屋心電圖是一個概念模擬，旨在將過時的iPhone重新用作監測建築物或橋梁結構勁度的工具。通過將iPhone粘在牆上並保持供電，該應用程式在地震期間記錄加速度數據。這些數據與氣象站數據同步，通過傅利葉轉換轉化為頻域信息，並存儲在數據庫中。每次地震的頻域信息與之前的記錄進行比較，以檢測結構勁度的變化。如果檢測到顯著變化，表明可能存在結構損壞，系統會通過電子郵件通知用戶，建議進行專業檢查。

### Concept / 概念

**English:**  
The core idea is to use the iPhone's accelerometer to capture earthquake duration data. If a structure's stiffness is theoretically infinite, its earthquake duration should match that of a meteorological station. By applying Fourier Transform to the recorded data, frequency domain information is obtained and logged. Comparing frequency domain data across multiple earthquakes helps identify changes in stiffness. A notable decrease in stiffness suggests structural damage, prompting a notification to the user for further inspection.

**中文:**  
核心理念是使用iPhone的加速度計捕捉地震歷時數據。如果結構的勁度理論上無限大，其地震歷時應與氣象站的數據一致。通過對記錄數據應用傅利葉轉換，獲得頻域信息並記錄下來。跨多次地震比較頻域數據有助於識別勁度的變化。勁度的顯著下降表明結構損壞，會觸發通知用戶進行進一步檢查。

### Simulated Case Study / 模擬案例研究

**English:**  
Consider monitoring a 3-story residential building with a theoretical natural frequency of about 3–5 Hz. The simulation process is as follows:  
- **Earthquake Occurrence**: The iPhone records acceleration duration, synchronized with data from a meteorological station (e.g., Taichung Station).  
- **Spectral Analysis**: The meteorological station spectrum shows peaks at 0.5 Hz and 2 Hz, while the iPhone spectrum shows peaks at 0.5 Hz, 2 Hz, and 4 Hz.  
- **Transfer Function**: The transfer function highlights a peak at 4 Hz, confirming it as the building's natural frequency.  
- **Multiple Earthquake Comparison**:  
  - First earthquake: Natural frequency at 4.0 Hz.  
  - Second earthquake: Natural frequency at 3.8 Hz (a 5% decrease).  
- **Trigger Warning**: Possible stiffness reduction detected, suggesting a structural inspection.

**中文:**  
假設監測一棟3層樓住宅，理論固有頻率約為3–5 Hz。模擬流程如下：  
- **地震發生**：iPhone記錄加速度歷時，與氣象站數據（例如台中氣象站）同步。  
- **頻譜分析**：氣象站頻譜顯示峰值在0.5 Hz和2 Hz，而iPhone頻譜顯示峰值在0.5 Hz、2 Hz和4 Hz。  
- **傳遞函數**：傳遞函數突出4 Hz的峰值，確認為房屋固有頻率。  
- **多次地震比對**：  
  - 第一次地震：固有頻率為4.0 Hz。  
  - 第二次地震：固有頻率為3.8 Hz（下降5%）。  
- **觸發警告**：可能檢測到勁度下降，建議檢查結構。

### Features / 功能

- **Real-Time Vibration Simulation / 即時振動模擬**: Displays a dynamic chart mimicking an ECG to show building vibration amplitude over time.  
  顯示一個動態圖表，模仿心電圖，展示建築物隨時間變化的振動幅度。
- **Structural Frequency Monitoring / 結構頻率監測**: Shows baseline and current structural frequencies to detect potential structural changes.  
  顯示基準和當前結構頻率，以檢測潛在的結構變化。
- **Earthquake Event Simulation / 地震事件模擬**: Allows users to trigger a simulated earthquake to observe the structural response and potential frequency drops.  
  允許用戶觸發模擬地震，觀察結構響應和可能的頻率下降。
- **Bilingual Interface / 雙語界面**: Available in both Chinese (中文) and English for user convenience.  
  提供中文和英文界面，方便用戶使用。

### Usage / 使用方法

**English:**  
1. Open `index.html` in a web browser to view the Chinese version, or `index_en.html` for the English version.  
2. Use the language selection menu in the top right corner to switch between languages.  
3. Click the "Simulate Earthquake Event" (or "模擬地震事件") button to trigger a simulation and observe changes in vibration and structural frequency.  
4. Monitor the status messages for analysis of the building's condition post-simulation.

**中文:**  
1. 在網頁瀏覽器中打開 `index.html` 查看中文版本，或打開 `index_en.html` 查看英文版本。  
2. 使用右上角的語言選擇選單切換語言。  
3. 點擊「模擬地震事件」（或 "Simulate Earthquake Event"）按鈕觸發模擬，觀察振動和結構頻率的變化。  
4. 查看狀態訊息，了解模擬後建築物狀況的分析。

### Files / 檔案

- `index.html`: The main file for the Chinese version of the simulation.  
  中文版本模擬的主檔案。
- `index_en.html`: The English version of the simulation.  
  英文版本的模擬檔案。

### Disclaimer / 免責聲明

**English:**  
This application is a conceptual demo for simulation purposes only and does not represent real structural health monitoring. It should not be used for actual building analysis or safety assessments.

**中文:**  
此應用程式僅為模擬用途的概念展示，不代表真實的結構健康監測。不應用於實際建築分析或安全評估。

### License / 許可證

© 2025 Structural Monitoring App Concept Demo. For demonstration purposes only.  
© 2025 結構監測App概念展示。僅供展示用途。
