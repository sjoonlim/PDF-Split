# PDF-Split

A simple Python tool to split a PDF file into multiple smaller PDF files, each containing a specified range of pages. This tool is useful when you want to break down large PDF documents into smaller, more manageable files. 

## Features

- Split a PDF into individual pages or custom ranges of pages.
- Easy to use with command-line interface.
- Outputs each split as a separate PDF file.

## Requirements

- Python 3.x
- `PyPDF2` library

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/yourusername/pdf-splitter.git
    cd pdf-splitter
    ```

2. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

You can split a PDF file into multiple PDF files using the command line. Here's how you can use the tool:

1. **Split by Individual Pages:**

    This will split the input PDF into single-page PDFs.

    ```bash
    python pdf_splitter.py input.pdf
    ```

    The script will create a new folder called `output` (if it doesn't exist) and save each page as a separate PDF file named `page_1.pdf`, `page_2.pdf`, etc.

2. **Split by Page Ranges:**

    You can also specify custom ranges of pages to split. For example, to split pages 1-3, 4-7, and 8-10:

    ```bash
    python pdf_splitter.py input.pdf 1-3 4-7 8-10
    ```

    Each specified range will be saved as a separate PDF file.

## Example

If you have a PDF called `document.pdf` and you want to split it into three parts: pages 1-3, 4-7, and 8-10, you would run:

```bash
python pdf_splitter.py document.pdf 1-3 4-7 8-10
