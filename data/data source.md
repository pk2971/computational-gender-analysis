# UK Parliament Debate Transcripts (TheyWorkForYou XML)

This repository documents the process of downloading **historical British Parliament debate transcripts** in XML format from [TheyWorkForYou.com](https://www.theyworkforyou.com/), which provides structured parliamentary data under open terms.

## Dataset Description

- **Source:** [TheyWorkForYou.com](https://www.theyworkforyou.com/)
- **Format:** XML files for each parliamentary sitting, organized by date
- **Contents:** Each file contains structured data on debates and speeches, suitable for parsing and analysis

## How to Download the Data

The data is publicly available via an `rsync` server. The following steps were performed on a Mac terminal:

### 1. Explore Available Datasets

To list available datasets on the remote server:

### 2. Download Debate XML Files

To mirror the **scraped XML files for debates** (excluding temporary and versioning files):

rsync -az --progress
--exclude '.svn'
--exclude 'tmp/'
--relative
data.theyworkforyou.com::parldata/scrapedxml/debates/
./parldata/


- `-a`: Archive mode (preserves permissions, timestamps, etc.)
- `-z`: Compress data during transfer
- `--progress`: Show download progress
- `--exclude`: Skip unwanted files and directories
- `--relative`: Preserve relative paths

> **Note:** This command will download all available debate XML files into a local `parldata/` directory, preserving the original structure.

## Example File Structure

After download, your directory will look like:

parldata/
scrapedxml/
debates/
debates1919-02-04a.xml
debates2020-09-23b.xml
...

## Usage

You can now parse or analyze the XML files using your preferred tools or scripts. For example, see [this blog post](https://blog.koheiw.net/?p=33) for R code to import and process the debates[2].

## License

Refer to [TheyWorkForYou.com](https://www.theyworkforyou.com/) for data usage terms.

---

*Last updated: July 5, 2025*


