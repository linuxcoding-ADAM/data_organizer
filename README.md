# 🗂️ Data Organizer

**A simple yet powerful Python script** that automatically organizes files in any folder based on their type (or extension).  
Useful for keeping your *Downloads*, *Desktop*, or *project folders* clean and structured.

---

## ⚙️ What This Script Does
The script scans a directory and automatically:
- Creates folders by file type (e.g. `Images`, `Videos`, `Documents`, `Audio`, `Archives`, etc.)
- Moves each file into its correct folder based on its extension
- Skips subfolders (won’t break your existing structure)
- Gracefully handles duplicate or read-only files
- Lets you organize multiple directories in one session

---

## 🧠 Example
### Before:
Downloads/
├── movie.mp4
├── photo.jpg
├── resume.docx
├── song.mp3
├── archive.zip



### After running the script:
Downloads/
├── Videos/
│ └── movie.mp4
├── Images/
│ └── photo.jpg
├── Documents/
│ └── resume.docx
├── Audio/
│ └── song.mp3
├── Archives/
│ └── archive.zip



## 🚀 How to Run

### 1️⃣ Clone or download this repository

git clone https://github.com/<your_username>/data_organizer.git
cd data_organizer

2️⃣ Run the script
bash
Copy code
python3 data_organizer.py
or (depending on your setup):
python data_organizer.py

3️⃣ Follow the on-screen prompts
Enter the path of the directory you want to organize.

You can add multiple directories in one run.

Press Enter on an empty line to start organizing.

Example:
Please enter a directory path to organize (or press Enter to finish): /home/adam/Downloads
Do you want to add another directory? (y/n): n
Starting organization for 1 directory...
Processing directory: /home/adam/Downloads
  Moved 'photo.jpg' to 'Images'
  Moved 'resume.docx' to 'Documents'
All tasks are complete.

🧩 Requirements
This script uses only standard Python libraries, no external installs needed:

os

shutil

✅ Works on Linux, macOS, and Windows.

🧰 Supported File Types
Category	Extensions
Images	.jpg, .jpeg, .png, .gif, .bmp, .tiff, .webp, .svg
Videos	.mp4, .avi, .mov, .mkv, .flv, .wmv
Audio	.mp3, .wav, .ogg, .flac, .aac
Documents	.pdf, .docx, .doc, .txt, .pptx, .xlsx, .csv
Archives	.zip, .rar, .tar, .gz
Executables / Installers	.exe, .msi
Disk Images	.iso
Other	Any unknown extensions go to an “Other” folder

⚠️ Safety Notes
The script moves files, it does not copy them.
(Files are safely transferred into subfolders within the same directory.)

If a file with the same name already exists in the target folder, it skips it and continues.

Run it on a test directory first if you want to see the behavior.
