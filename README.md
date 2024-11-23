# Media Converter

A screen reader-friendly desktop application for converting audio and video files between different formats. Built with Python and wxPython, using FFmpeg for media conversion.

## Features

- Convert between popular video and audio formats
- Native Windows controls for optimal accessibility
- Full screen reader support with NVDA and JAWS
- Keyboard shortcuts for all major functions
- Progress tracking during conversion
- Error handling with accessible notifications
- Help system with keyboard navigation guide

## Supported Formats

### Video Formats
- MP4 (.mp4)
- AVI (.avi)
- MKV (.mkv)
- MOV (.mov)
- WMV (.wmv)

### Audio Formats
- MP3 (.mp3)
- WAV (.wav)
- AAC (.aac)
- OGG (.ogg)
- FLAC (.flac)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Orinks/Media-Converter.git
cd Media-Converter
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

4. Install FFmpeg:
   - Windows: Download from [FFmpeg website](https://ffmpeg.org/download.html) and add to PATH
   - Linux: `sudo apt-get install ffmpeg`
   - macOS: `brew install ffmpeg`

## Usage

1. Run the application:
```bash
python media_converter/main.py
```

2. Select an input file using the "Browse" button or press Ctrl+O
3. Choose the desired output format from the dropdown menu
4. Click "Convert" or press Ctrl+C to start the conversion
5. Select the output location when prompted
6. Wait for the conversion to complete

### Keyboard Shortcuts

- `Ctrl+O`: Open file selection dialog
- `Ctrl+C`: Start conversion
- `F1`: Show help with keyboard navigation guide
- `Tab`: Navigate between controls
- `Space/Enter`: Activate buttons and controls
- `Escape`: Close dialogs

## Accessibility Features

- Native Windows controls for optimal screen reader compatibility
- Full keyboard navigation support
- Clear focus indicators
- Descriptive labels and announcements
- Help system with navigation guide
- Standard Windows keyboard behavior

## Requirements

- Python 3.6 or higher
- FFmpeg
- Required Python packages (see requirements.txt):
  - wxPython
  - ffmpeg-python

## Project Structure

```
media_converter/
├── converter.py     # Core conversion logic
├── gui.py          # User interface implementation
├── main.py         # Application entry point
└── requirements.txt # Project dependencies
```

## Error Handling

The application includes comprehensive error handling for:
- Unsupported file formats
- Invalid input files
- Failed conversions
- FFmpeg errors

All errors are reported through native Windows dialogs for optimal accessibility.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

[MIT License](LICENSE)

## Acknowledgments

- FFmpeg for media conversion capabilities
- wxPython for the accessible GUI framework
