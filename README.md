# SukuAI
SukuAI เป็นโปรแกรม AI ที่ทำงาน บนเครื่องของคุณแบบ offline ช่วยให้คุณพิมพ์ข้อความได้อย่าง ราบรื่นและถูกต้องแม้ลืมเปลี่ยนภาษา โดยรองรับการแปลงเค้าโครงแป้นพิมพ์ ไทย ↔ อังกฤษ และแก้คำผิดในเวลาเดียวกัน

You are an AI coding assistant. Your task is to generate a **full working desktop application** that runs **offline** to automatically correct and convert text typed in **Thai ↔ English**.

Requirements:

1. **Functionality**:
   - Detect keyboard layout mismatch (Thai ↔ English)
   - Automatically convert the text to the correct layout
   - Auto-correct words in real-time for both Thai and English
   - Handle multi-character input, backspace, and cursor position
   - Work completely offline without internet
   - Learn user typing habits to improve suggestions over time

2. **Frontend (GUI)**:
   - Use **HTML + CSS + JavaScript** for the interface
   - Modern and minimalistic design: input box, suggestion popup, toggle switches
   - Realtime display of corrected text and suggestions
   - Optional settings panel to enable/disable auto-correct or toggle layout

3. **Backend (AI logic)**:
   - Written in **Python**
   - Use `pynput` or `keyboard` for keyboard input hooks
   - Use dictionary-based auto-correct and/or tiny AI model offline (e.g., fastText, TinyBERT)
   - Include mapping dictionaries for Thai ↔ English keyboard layouts
   - Communicate with frontend via **IPC / WebSocket / local server** to display corrections in real-time

4. **Project Structure**:
   - `main.py` → starts Python backend
   - `mapping_engine.py` → layout conversion logic
   - `auto_correct.py` → spell correction and AI logic
   - `frontend/` → contains `index.html`, `style.css`, `app.js` for GUI
   - Instructions to package as a desktop app using **Electron** or **PyInstaller + local web view**

5. **Output Requirements**:
   - Fully working code for backend and frontend
   - Clear comments in all files
   - Instructions to run on Windows and Linux
   - Use offline dictionary / model files included in project

6. **Extra Features**:
   - Display suggestion popup under the input box
   - Animate popup smoothly (fade in/out)
   - Highlight corrected words
   - Optional dark/light mode toggle

Generate **all necessary files** and **full code** according to this specification so it can run offline and provide a modern, interactive GUI for the AI typing assistant.

