# ⏱️ Stopwatch Project

A clean, modern, and fully functional **Stopwatch Application** built with **HTML, Tailwind CSS, and JavaScript**.  
It supports start, stop, reset, millisecond accuracy, and previous-record saving — all inside a smooth UI.

---

## 📸 Preview  
<img width="1919" height="908" alt="image" src="https://github.com/user-attachments/assets/5fdf6c93-c4ed-4e63-a87b-677fdf0dc7c0" />


---

## 🌟 Features

- 🟢 **Start**, 🟡 **Stop**, 🔴 **Reset** buttons  
- ⏱️ **Millisecond-level stopwatch**  
- 📝 Saves every stopped time into a list  
- 🧹 Reset clears both timer and saved records  
- 🎨 Tailwind CSS styling  
- 📱 Fully responsive  
- ⚡ Smooth interval updates (10ms)

---

## 🛠️ Tech Stack

- **HTML5** — Structure  
- **Tailwind CSS** — Styling  
- **JavaScript** — Timer functionality & DOM updates  

---

## 📁 Project Structure

stopWatch/
│── index.html
│── README.md

yaml
Copy code

---

## 🔧 How It Works

### 🏃 Start Timer
```js
timerId = setInterval(startTimer, 10);
✋ Stop Timer (also saves record)
js
Copy code
clearInterval(timerId);
timerId = null;
progressSave(timerDisplay.innerText);
🔁 Reset Timer + Clear Records
js
Copy code
clearProgressSave();
timerDisplay.innerHTML = "00:00:00";
⏱️ Timer Logic (10ms interval)
js
Copy code
millisecond++;
if (millisecond == 100) {
    millisecond = 0;
    second++;
    if (second == 60) {
        second = 0;
        minute++;
    }
}
🚀 Getting Started
1️⃣ Clone this repository
bash
Copy code
git clone https://github.com/abeerpathela/stopWatch.git
2️⃣ Open the folder
bash
Copy code
cd stopWatch
3️⃣ Run the project
Open index.html in your browser.

🤝 Contributing
PRs and suggestions are welcome!

👨‍💻 Author
Made with ❤️ by Abeer Pathela

yaml
Copy code

---

If you want, I can also:

🎨 Add screenshot  
🏷️ Add badges  
✨ Add a colorful design  
📦 Add more documentation  

Just tell me!
