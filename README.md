# 🔽 4-bit Down Counter with Enable & Reset (Verilog)

This project implements a **4-bit Down Counter** in Verilog with **Enable** and **Reset** functionality.  
The counter decrements its value on each positive edge of the clock when `enable = 1`.  
If `reset = 1`, the counter resets to `1111` (15 in decimal).

---

## 📌 Features
- 4-bit down counter (counts `1111` → `0000` → wraps back to `1111`)
- **Enable input** to control counting
- **Asynchronous Reset** to set the counter back to `1111`
- Synchronous operation on positive clock edge
- Verified using **testbench** with console output and waveform (EPWave)

---

## 🛠 Files Included
- `txt file` → Verilog module for 4-bit down counter  and Testbench with clock, reset, enable control, and waveform dump  
- `waveform file` → Waveform file (generated after simulation, view in EPWave)  

---

## ▶️ Simulation Steps (EDA Playground)
1. Open [EDA Playground](https://www.edaplayground.com/).  
2. Create a new project and paste:  
   - `code` in **Design file**  
   - `testbench` in **Testbench file**  
3. Select a simulator (e.g., **Icarus Verilog**).  
4. Enable **EPWave** (waveform viewer).  
5. Click **Run**.  

---

## 📊 Console Output (Tabular Form)

| Time (ns) | Reset | Enable | Count (Binary) | Count (Decimal) |
|-----------|-------|--------|----------------|-----------------|
| 0         | 1     | 0      | 1111           | 15 |
| 10        | 0     | 0      | 1111           | 15 |
| 20        | 0     | 1      | 1110           | 14 |
| 30        | 0     | 1      | 1101           | 13 |
| 40        | 0     | 1      | 1100           | 12 |
| 50        | 0     | 1      | 1011           | 11 |
| 60        | 0     | 1      | 1010           | 10 |
| 70        | 0     | 1      | 1001           | 9 |
| 80        | 0     | 1      | 1000           | 8 |
| 90        | 0     | 1      | 0111           | 7 |
| 100       | 0     | 1      | 0110           | 6 |
| 110       | 0     | 0      | 0110           | 6 |
| 140       | 0     | 1      | 0101           | 5 |
| 150       | 1     | 1      | 1111           | 15 |
| 160       | 0     | 1      | 1110           | 14 |
| 170       | 0     | 1      | 1101           | 13 |
| 180       | 0     | 1      | 1100           | 12 |

---

## 📉 Waveform (EPWave)
You should see:
- **Clock** toggling  
- **Reset** asserted and released  
- **Enable** controlling the counter  
- **Count** decreasing from `1111` down to `0000`, then rolling back  

---

## ✅ Learning Outcomes
- Understand **Flip-Flops** and sequential circuits  
- Learn **Clock handling** in Verilog  
- Implement **Enable** and **Reset** in counters  
- Generate and analyze **waveforms** using EPWave  

---
