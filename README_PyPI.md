# klctool - Karaoke Lyrics Card Creation Support Tool

![sample image](https://raw.githubusercontent.com/AmasaShiro/klctool/refs/heads/main/resources/sample.jpeg)

- klctool: Command Line tool
  - Hiragana conversion of lyrics: Powered by Google Gemini
  - Conversion to word processor format - ODT format for LibreOffice Writer using Pandoc
  - Background image processing: Adjusts images for use as lyrics card backgrounds

## Documentation

[Japanese](https://github.com/AmasaShiro/klctool/blob/main/README.md)  
[English](https://github.com/AmasaShiro/klctool/blob/main/README_en.md)

## Prerequisites

- Python
- Pandoc
- LibreOffice Writer

- Google Gemini API Key

## Installation

```zsh
pip install klctool
```

## Usage examples

```shell
klctool hiragana lyrics_file_name
klctool convert2odt lyrics_file_name_hiragana
klctool adjustimage image_file_name1 image_file_name2
```

## Customization

- Configuration file location:
  - macOS / Linux: ~/.config/klctool/
  - Windows: %APPDATA%

```zsh
.config
└── klctool
    ├── config.toml  # Default configuration values, etc.
    ├── gemini-2.0-flash-exp.api_key.toml  # API key
    ├── gemini-2.0-flash-exp.prompt.toml   # Prompt
    ├── klctool-edit.lua # Lua script for Pandoc
    ├── klctool.odt      # ODT template file
    └── paper-size.toml # Paper size definitions
```

## License

MIT License

## Development / Test Environment

- MacBook Air Retina, 13-inch, 2018 Intel
- MacOS Sonoma 14.7.4
- Python 3.13.2
- Pandoc 3.6.4
- LibreOffice Version: 25.2.1.2 (X86_64) / LibreOffice Community / Japanese Language Pack

## Acknowledgements

- The code was basically written by Google Gemini. It was very helpful and I am grateful!
- Thank you to all OSS developers!
