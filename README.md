# ALSD 2 Mini Project

---

## 📝 Description

A basic word puzzle game prototype where players form valid words from given letters to progress through levels.

**Windows users:** Just run the `.exe` file, or use the `.bat` file to build and run the game.

### Core Mechanics

* 10 levels with increasing difficulty
* Words must be 2–6 letters long
* Dictionary validation using a provided word list
* Simple user account system

---

## 📦 Folder Structure

```text
LSD-2-Mini-Project-/
├── compiler/                  # MinGW-w64 GCC 13.2.0 (from winlibs)
│   └── bin/
│       ├── gcc.exe            # C compiler
│       ├── g++.exe            # C++ compiler (if needed)
│       ├── ar.exe             # Archiver
│       ├── libwinpthread-1.dll # Required DLL
│       └── ...                # Other necessary files (lib/, include/, etc.)
├── include/                   # Raylib + RayGUI headers
│   ├── raylib.h
│   └── raygui.h
├── libs/                      # Static libraries
│   └── libraylib.a
├── src/                        # Game source code
│   └── main.c
├── words.txt                   # Dictionary file
├── game.exe                    # Compiled output
├── build.bat                   # One-click build script
├── users/                      # Created at runtime
│   └── *.dat                   # User save files
├── .gitignore                  # Git ignore file
└── README.md                   # Project documentation
```

---

## ⚙️ Installation & Setup

Everything is portable on Windows.

### Compile & Run the Game

1. Open the project folder.
2. Run `build.bat` to compile and launch the game.

---

## 🎮 How to Play

### 1. User Setup

* Register a new account or log in.
* Usernames are case-sensitive.

### 2. Gameplay

Each level provides a set of letters. Form words that:

* Use only the provided letters.
* Contain between 2 and 6 letters.
* Exist in the dictionary.

Complete all required words to advance through the 10 levels. Your progress is saved automatically.

---

## 🔧 Technical Details

* **Libraries:** Raylib 4.5 (graphics/input), RayGUI 3.2 (UI components).
* **Core Functions:** Dictionary loading and validation, level configuration, and user data persistence.
* **Dictionary:** The `words.txt` file may take a long time to load because of its size.
* **Limitations:** No error handling for missing files, fixed window size (800 × 600), and a basic UI without animations.

---

## 📌 Notes

* **Version:** Prototype (v0.0.1) for educational purposes.
* **License:** No license. For ALSD 2 (Algorithm et Structure des Données) course use only.
* **Custom Dictionaries:** The `words.txt` file can be replaced with custom word lists.
* **Game Assets:** All game assets are included in the repository.

---

## 🎓 Developed For

* Algorithm et Structure des Données (ALSD) course
* Computer Engineering Department
* University of Bejaia

---

## 🛑 Report Issues

If you encounter any bugs or errors, please open an issue in this repository or contact the developer.
