# ASCII VIDEO

ASCII VIDEO is a Python application that converts videos into animated ASCII art directly in your terminal. It supports real-time playback, colored ASCII rendering, multi-language menus, and exporting ASCII animations as MP4 videos.

---

## Features

- Real-time ASCII video playback in the terminal
- Optional colored ASCII rendering
- Multi-language support
  - English
  - Spanish
  - French
  - Portuguese
  - German
  - Bahasa
- Automatic terminal size detection
- Adjustable output width
- Frame skipping for performance optimization
- Loop playback mode
- Export ASCII animation to MP4
- Save or delete generated PNG frames
- Custom background colors during export

---

## Requirements

Before running the application, install:

- Python 3.9 or newer
- OpenCV
- NumPy
- Pillow

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Demon69i/ascii-video.git
cd ascii-video
```

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install opencv-python numpy Pillow
```

---

## requirements.txt

Create a file named `requirements.txt` and add:

```txt
opencv-python
numpy
Pillow
```

---

## Running the Application

Run:

```bash
python ASCII_v5_official.py
```

---

## How to Use

### Step 1: Select Language

When the application starts, choose one of the supported languages.

### Step 2: Enter Video Path

Enter the full path to your video file.

Example (Windows):

```text
C:\Users\YourName\Videos\sample.mp4
```

Example (Linux):

```text
/home/user/videos/sample.mp4
```

Example (macOS):

```text
/Users/user/Videos/sample.mp4
```

### Step 3: Enable Color Mode

Choose whether ASCII characters should use the original video colors.

Example:

```text
Character color? (y/N):
```

### Step 4: Set Output Width

Specify the width of the ASCII output.

Leave blank for automatic sizing.

Example:

```text
Output width (blank for Auto):
```

### Step 5: Configure Frame Skipping

Frame skipping improves performance.

Examples:

```text
1 = Show every frame
2 = Show every second frame
3 = Show every third frame
```

### Step 6: Loop Playback

Choose whether the preview should restart automatically after finishing.

### Step 7: Export to MP4

After playback finishes, you can export the ASCII animation as an MP4 video.

Options:

- MP4 only
- MP4 + PNG frame sequence

---

## Export Options

### Background Colors

Available backgrounds:

1. Black
2. White
3. Blue
4. Custom HEX color

Example:

```text
#FF0000
```

for a red background.

---

## Project Structure

```text
ascii-video/
│
├── ASCII_v5_official.py
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Recommended .gitignore

Create a file named `.gitignore`:

```gitignore
__pycache__/
*.pyc
*.pyo
*.pyd

venv/
.env

.vscode/

temp_ascii_frames/

*.png
*.mp4
```

---

## Example Workflow

1. Start the application.
2. Select English.
3. Enter a video path.
4. Enable color mode.
5. Choose automatic width.
6. Set frame skip to 1.
7. Preview the ASCII animation.
8. Export to MP4.
9. Save only the final MP4 file.

---

## Dependencies

This project uses:

- OpenCV (`opencv-python`)
- NumPy (`numpy`)
- Pillow (`Pillow`)

---

## Known Limitations

- Large videos may require significant disk space during export.
- Export speed depends on CPU performance.
- Very large terminal widths can reduce playback performance.
- Font availability may vary by operating system.

---

## Troubleshooting

### File Not Found

Make sure the video path is correct.

Example:

```text
File not found
```

Verify the file exists and use the full path.

### Missing Module Errors

Install dependencies:

```bash
pip install -r requirements.txt
```

### Video Does Not Play

Verify:

- Video file exists
- OpenCV is installed
- Supported video codec is available

### Export Fails

Ensure:

- Destination folder exists
- Sufficient disk space is available
- Video file can be opened by OpenCV

---

## Credits

Original Concept:

- Stepanussaruran

Enhanced Version:

- Nicolas Romero (CoralGamer)

Repository Maintainer:

- Demon69i

---

## License

This project is released under the MIT License.

You are free to use, modify, distribute, and improve the software.

---

## Support

If you encounter issues:

1. Verify Python installation.
2. Verify dependencies are installed.
3. Check the video path.
4. Check available disk space.
5. Ensure your terminal supports ANSI colors.

Enjoy using ASCII VIDEO.
