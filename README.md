🗂️ Data Organizer

A smart and minimal Python script that keeps your folders clean and organized automatically.
It scans any directory and sorts files into categorized subfolders based on their type or extension.

🚀 Overview

Tired of a messy Downloads or Desktop folder full of mixed files?
This script automatically:

Detects file types

Creates folders like Images, Videos, Documents, etc.

Moves files into their correct place

Handles duplicates safely

Works on any OS (Linux, macOS, Windows)

No dependencies, no setup — pure Python automation.

⚙️ Features

✅ Sorts files by type (image, video, audio, document, etc.)
✅ Automatically creates destination folders
✅ Skips folders (won’t move your directories)
✅ Works on multiple directories in one session
✅ Handles duplicate files gracefully
✅ Uses only Python’s built-in modules (os, shutil)
✅ Safe to run multiple times

🧩 Supported File Types
Category	Extensions
Images	.jpg, .jpeg, .png, .gif, .bmp, .tiff, .webp, .svg
Videos	.mp4, .avi, .mov, .mkv, .flv, .wmv
Audio	.mp3, .wav, .ogg, .flac, .aac
Documents	.pdf, .docx, .doc, .txt, .pptx, .xlsx, .csv
Archives	.zip, .rar, .tar, .gz
Executables / Installers	.exe, .msi
Disk Images	.iso
Other	Files with unknown extensions
🧠 Example
Before:
Downloads/
├── photo.jpg
├── resume.docx
├── video.mp4
├── archive.zip
├── song.mp3

After running the script:
Downloads/
├── Images/
│   └── photo.jpg
├── Documents/
│   └── resume.docx
├── Videos/
│   └── video.mp4
├── Archives/
│   └── archive.zip
├── Audio/
│   └── song.mp3

🧰 Requirements

✅ Works out of the box with Python 3+
No need to install anything extra — it only uses:

import os
import shutil

💻 How to Run

Clone or download this repository:

git clone https://github.com/linuxcoding-ADAM/data_organizer.git
cd data_organizer


Run the script:

python3 data_organizer.py


or (depending on your system)

python data_organizer.py


Follow the on-screen instructions:

Enter a directory path (like /home/adam/Downloads)

Add multiple paths if you want

Press Enter on an empty line to start organizing

🧾 Example Output
Please enter a directory path to organize (or press Enter to finish): /home/adam/Downloads
Do you want to add another directory? (y/n): n

Starting organization for 1 directory...
Processing directory: /home/adam/Downloads
  Created directory: /home/adam/Downloads/Images
  Moved 'photo.jpg' to 'Images'
  Moved 'resume.docx' to 'Documents'
  Moved 'video.mp4' to 'Videos'
  Moved 'archive.zip' to 'Archives'
  Moved 'song.mp3' to 'Audio'
All tasks are complete.

⚠️ Notes & Safety

The script moves files, not copies them (faster, no duplicates).

If a file already exists in the destination folder, it skips it.

You can run it safely multiple times — it won’t break your folders.

Test on a small directory first if you’re curious how it behaves.
