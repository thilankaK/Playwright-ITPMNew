# Test Automation

Short test automation project for running web-based test cases using `test_automation.py`.

## Overview

This repository contains a test runner script that reads test cases from an Excel file and runs browser-based automation against a target URL.

## Prerequisites

- Python 3.8 or newer
- Recommended: create and use a virtual environment
- Install dependencies (if any) with:

```
pip install -r requirements.txt
```

If there is no `requirements.txt`, ensure required packages such as `playwright` or `selenium` are installed as used by the project.

## Usage

Run the test runner with command-line arguments. Example (from recent usage):

```
python test_automation.py --excel "test_automation/Assignment 1 - Test cases.xlsx" \
  --url "https://www.pixelssuite.com/chat-translator" \
  --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --headless
```

Options may include Excel path, target URL, timing controls, and headless toggle. Check the script's `--help` for full options:

```
python test_automation.py --help
```

## Troubleshooting

- If the browser fails to start, ensure browser drivers or Playwright browsers are installed.
- For flaky timings, increase `--wait-ms` or `--type-delay-ms`.

## Contact

If you want additional help updating this README or adding examples, open an issue or contact the project maintainer.
