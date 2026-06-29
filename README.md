# pinnacle-records
A student &amp; teacher management system with a UI that doesn't look like a school project.  Built on a clean Python OOP backend (ABC, inheritance, JSON persistence) and wrapped in a navy-and-gold web interface with a 3D intro animation, live search, and color-coded grading.
Why this exists

Most "student management system" repos on GitHub are a while True loop, a print() menu, and a .json file. They work, but nobody wants to look at them twice.

Pinnacle Records takes that same idea — register students and teachers, track grades, look someone up — and gives it an interface people actually want to open. The backend is still simple, readable Python (great for anyone learning OOP/abstract classes). The frontend is the part that makes people stop scrolling.

✨ Features


🎬 3D pop-in intro — the app's "report card" rotates and pops out of the screen on load, like a flipped-open notebook
🟡 Gold-and-navy academic theme — not another templated cream-and-serif AI design
🔍 Live search — instantly filter students by name/roll, teachers by name/subject/ID
🏷️ Color-coded grading — automatic letter grades (A/B/C/F) with a circular average-progress ring per student
🧱 Clean OOP backend — Persons abstract base class, Student and Teacher subclasses, static email validation
💾 JSON persistence — no database setup, just a school_data.json file
🚫 Duplicate protection — won't let you register the same roll number or employee ID twice


🖥️ Tech stack

LayerTechBackend logicPython 3, abc module, JSONFrontendHTML5, CSS3 (custom properties, 3D transforms), vanilla JSFontsFraunces (display), Inter (body), JetBrains Mono (data)StorageFlat-file JSON (swap in SQLite/Postgres easily)

🚀 Quick start

bashgit clone https://github.com/<your-username>/pinnacle-records.git
cd pinnacle-records

# Run the CLI version
python school_manager.py

# Or just open the UI — no install needed
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux

No dependencies. No build step. That's intentional.

📂 Project structure

pinnacle-records/
├── school_manager.py   # CLI backend — Student/Teacher classes, JSON storage
├── index.html          # Frontend UI (intro animation, dashboard, rosters)
├── school_data.json    # Auto-generated on first run
└── README.md

🧭 Roadmap


 Flask API to connect the UI directly to school_manager.py (live persistence instead of in-memory)
 Login/role system (admin vs teacher vs student view)
 Export report cards as PDF
 Attendance tracking
 Dark mode toggle



Want to tackle one of these? Check Contributing below — first-timers welcome.



🤝 Contributing

This started as a learning project and is now open for anyone to extend. If you're new to open source, this is a good first repo:


Fork it
Create a branch: git checkout -b feature/attendance-tracker
Commit: git commit -m "Add attendance tracker"
Push and open a PR


Issues tagged good first issue are a solid place to start once they're up.



<div align="center">
If this saved you from writing another boring CLI school system, star the repo ⭐ — it helps other people find it too.

</div>
*The backend logic is hand-written Python (OOP fundamentals). The frontend UI was built with AI assistance and refined for this project.


