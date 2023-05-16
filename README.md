# Subtitle Processor

This Python script processes `.srt` (SubRip Text) files. It is designed to remove timestamps from these files, which are a common format for subtitles or captions, and output the resulting text.

## Requirements

- Python 3
- `pysrt` library for handling .srt files

To install the required library, run:

pip install pysrt


## Usage

You can use this script to process either all .srt files in the 'Subtitles' directory or a specific .srt file. 

If you're processing all files, you have the option to either concatenate all the text into one file or write each file's text into a separate output file.

Here's how to use the script:

python subtitle_processor.py [-a | --all] [-s | --single] [-f | --file filename]


### Options:

- `-a` or `--all`: Process all .srt files in the 'Subtitles' directory.
- `-s` or `--single`: When processing all files, use this option to output all text to a single file.
- `-f` or `--file` followed by a filename: Process a specific .srt file in the 'Subtitles' directory.

### Examples:

1. To process all .srt files and output each file's text to a separate output file:

python subtitle_processor.py --all


2. To process all .srt files and concatenate all text into a single file:

python subtitle_processor.py --all --single


3. To process a specific .srt file:

python subtitle_processor.py --file filename.srt

