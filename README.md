# Paper Recommender

A lightweight Python recommendation prototype that fetches real research paper metadata from Crossref and suggests papers based on your query and feedback.

## Features

- Uses live Crossref paper metadata by default
- Presents one paper at a time in the terminal
- Supports user feedback: accept, reject, save for later
- Builds a simple interest profile from accepted papers
- Includes an offline `--local` mode if you want to run without network access

## Requirements

- Python 3.8 or newer

## Usage

Run from the project folder:

```bash
C:/Users/gaiya/AppData/Local/Programs/Python/Python313/python.exe paper_recommenderss.py "machine learning"
```

Or run with no query to be prompted:

```bash
C:/Users/gaiya/AppData/Local/Programs/Python/Python313/python.exe paper_recommenderss.py
```

### Optional offline mode

If you want to use the local database instead of live Crossref data:

```bash
C:/Users/gaiya/AppData/Local/Programs/Python/Python313/python.exe paper_recommenderss.py --local "machine learning"
```

## Commands while running

- `y` / `yes` — accept the paper
- `n` / `no` — reject the paper
- `s` / `save` / `later` — save for later
- `l` / `list` — show saved reading list
- `p` / `profile` — show feedback summary
- `q` / `quit` / `exit` — quit the program

## Notes

- Live Crossref fetching is the default.
- If live fetching fails, the script falls back to a local paper database with real paper metadata.
- `index.html` is provided for static GitHub Pages documentation.
