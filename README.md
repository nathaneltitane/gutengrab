![dextop](https://raw.githubusercontent.com/nathaneltitane/gutengrab/main/gutengrab.svg)

[![Donate](https://img.shields.io/badge/Paypal-2f343f.svg?style=for-the-badge&logo=paypal&label=Donate)](https://www.paypal.com/donate?hosted_button_id=ZW3CDCANHJCWJ)

[[ GutenGrab // Project Page ]](https://github.com/nathaneltitane/gutengrab) [ Version // 11-07-2025 ]


---

### NOTICE

11-07-2025 ↴

- Update readme

---

### Welcome to GutenGrab

GutenGrab, the Gutendex API / Project Gutenberg Terminal Interface: access the project's book catalog via the Gutendex API, stright from your terminal emulator!

With GutenGrab, you can:

- Search for books by title, author, or subject (with optional language filtering).
- View book details, including:
  - title, author, languages, subjects, and available formats.
- List all available download formats:
  - EPUB, MOBI, TXT, HTML, etc.
- Download books in EPUB format (for now).
- Save and reuse search results:
  - download all books from the last search using  the 'all' argument'.

---

### TL;DR

GutenGrab is a Bash terminal client for Gutendex — an API for Project Gutenberg’s public-domain book catalog.

It lets you search, inspect, and download eBooks directly from your terminal, with built-in language filtering, rich book info display, and support for multi-book downloads.

The script automatically installs and manages what it needs:

- curl
- jq
- frobulator (auto-downloaded to ~/.local/bin/frobulator if missing)

Clone the repository ↴

```
git clone https://github.com/nathaneltitane/gutengrab.git
```

Move into the directory ↴

```
cd gutengrab
```

Make it executable ↴

```
chmod +x gutengrab
```

Run it ↴

```
bash gutengrab
```

Note:

can also be installed globally:

```
sudo install -m 755 gutengrab /usr/local/bin/gutengrab
```

---

### Features

- Search books by title, author, or subject
- Filter by language (e.g. en, fr, es)
- View details: title, author, subjects, and formats
- Download EPUB books directly
- Batch download using all to fetch every result from your last query
- Interactive TUI with colorized feedback (uses frobulator)

---

### Usage

Once launched, GutenGrab presents a menu of actions:

```
[ 1 ] [S]earch for a book           [ author | title | subject ]
[ 2 ] [G]et book details            [ id ]
[ 3 ] [D]ownload book(s) (epub)     [ id ]
[ 4 ] [E]xit
```

### Search

Enter a keyword (alphanumeric), for example:

```
[ + ] Enter search query [ author / title / subject ]: pride
[ + ] Enter language - [ ↵ ] to skip [ en / fr / es / .. ]: en
```

Results are fetched from Gutendex and displayed in a readable format with IDs, titles, authors, and EPUB links.

---

### Book Details

To fetch detailed info about a book:

```
[ + ] Enter book identifier: 1342
```

Outputs title, author, subjects, and available download formats.

---

### Download Book(s)

You can download:

- One or multiple books by ID:

  ```
  [ + ] Enter Book identifier(s): 1342 84
  ```

- All books from your last search:

  ```
  [ + ] Enter Book identifier(s): all
  ```

Downloaded files are saved in your current directory as:

```
<Author> - <Title>.epub
```

---

## API Reference

Uses the public [Gutendex API](https://gutendex.com/books) for:

- `/books/?search={query}`
- `/books/{id}/`
- Supports all [ISO-639-1 language codes](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
- Integrates seamlessly with frobulator for interface styling and error handling
- Tested on Debian-based systems (Termux compatible)

---

### Reports:

[Submit bug report or feature request](https://github.com/nathaneltitane/gutengrab/issues)

### Projects:

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/dextop?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=DEXTOP)](https://github.com/nathaneltitane/dextop)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/frobulator?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=FROBULATOR)](https://github.com/nathaneltitane/frobulator)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/gutengrab?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=GutenGrab)](https://github.com/nathaneltitane/gutengrab)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/l2cu?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=L²CU)](https://github.com/nathaneltitane/l2cu)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/terminal?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=TERMINAL)](https://github.com/nathaneltitane/terminal)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/mechablocks?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=MECHA%20//%20BLOCKS)](https://github.com/nathaneltitane/mechablocks)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/pixtrm?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=PIXTRM)](https://github.com/nathaneltitane/pixtrm)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/nathaneltitane?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=NATHANEL%20%2b%20TITANE)](https://github.com/nathaneltitane/nathaneltitane)

[![GitHub Repo stars](https://img.shields.io/github/stars/nathaneltitane/pewpewprints?style=for-the-badge&logo=gnubash&logoColor=ffffff&label=PEW%21%20PEW%21%20PRINTS)](https://github.com/nathaneltitane/pewpewprints)

---

[[ GutenGrab // Project Page ]](https://github.com/nathaneltitane/gutengrab) [ Version // 11-07-2025 ]

### Enjoying Dextop? Buy me a coffee to show your appreciation!

[![Donate](https://img.shields.io/badge/Paypal-2f343f.svg?style=for-the-badge&logo=paypal&label=Donate)](https://www.paypal.com/donate?hosted_button_id=ZW3CDCANHJCWJ)
