# 🔧 G-Code to Drawing object (CAD) Converter

An integrated CNC toolpath visualization project combining an Excel-based G-code parser with a ZVB macro visualizer for use in ZWCAD/AutoCAD environments.

## 🚀 Features
- 🧠 Parses G-code from Excel including G0, G1, G2/G3 arcs
- 🧾 Computes START and END coordinates per movement
- 📋 Generates structured data for visualization: `X1,Y1,Z1,X2,Y2,Z2,isRapid`
- 🖥️ Visualizes movement in ZVB using lines and arcs with color logic
- 🔴 Red indicator lines for start and end of toolpath

## 🧩 How It Works
1. Open `TRIAL_PARSING_TOOL.xlsm` in Excel  
2. Paste your G-code into the designated sheet  
3. `FINAL DATA` will be generated automatically  
4. Copy all rows from the `FINAL DATA` column  
5. Open **ZWCAD**, then:
   - Run `LOAD` to load the ZVB_Visualizer.zvb macro
   - Run `VBARUN`, choose `cmdDrawLines_Click`
6. Paste the data into the input box
7. Click **Submit / Draw**
8. Visualized toolpath will appear in model space

## 🧑‍💻 Author
**Galih Primananda**  
[LinkedIn](https://www.linkedin.com/in/galihprime) • [Instagram](https://www.instagram.com/glh_prima)


