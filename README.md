# FakeFileMaker

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

A simple Python tool for creating fake files of specified sizes. Useful for testing file handling, disk space simulation, or creating placeholder files for development purposes.

## Features

- Create files of any specified size
- Support for both KB and MB size units
- Interactive command-line interface
- Prevents overwriting existing files
- ASCII art banner for a friendly user experience

## Requirements

- Python 3.x (all versions)
- No external dependencies required

## Installation

1. Clone or download this repository:
   ```bash
   git clone <repository-url>
   cd FakeFileMaker
   ```

2. No additional installation required - just run the script!

## Usage

Run the script using Python:

```bash
python fakeFileMaker.py
```

The program will prompt you for:

1. **File name**: Enter the full name of the file you want to create (including extension)
2. **Size unit**: Choose between:
   - `MG` (Megabytes)
   - `KB` (Kilobytes)
3. **Size**: Enter the numeric size value

### Example

```
Enter Fullname of file: test_file.txt
Enter mode (MG, KB): MB
Enter size as mg: 5
```

This will create a 5MB file named `test_file.txt` in the current directory.

## How It Works

The tool creates files by writing repeated 'A' characters:
- For MB files: writes `size × 1,000,000` bytes
- For KB files: writes `size × 1,000` bytes

## Safety Features

- **File existence check**: The program will not overwrite existing files
- **Error handling**: Exits gracefully if a file with the same name already exists

## Use Cases

- **Testing**: Create files of specific sizes for testing file handling code
- **Development**: Generate placeholder files for development environments
- **Disk space simulation**: Quickly fill up disk space for testing purposes
- **Performance testing**: Create large files to test application performance

## Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## License

This project is open source and available under the [MIT License](LICENSE).
