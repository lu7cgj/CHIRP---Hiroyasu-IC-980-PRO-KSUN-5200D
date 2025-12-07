## ☕ Donate

If you find these tools useful and want to support my work, you can donate here:

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/donate?business=gcamji%40gmail.com&currency_code=USD)


🛰️ CHIRP ↔ Hiroyasu IC-980Pro Converter Toolkit

This repository provides a simple, reliable bridge between CHIRP and the Hiroyasu IC-980Pro (and other rebranded models using the same YSF codeplug format).

CHIRP does not natively support Hiroyasu radios, and the official CPS software is slow, limited, and difficult to edit.
This toolkit solves that problem by allowing:

✔ CHIRP CSV → YSF codeplug

✔ YSF codeplug → CHIRP-compatible CSV

With these two scripts you can fully edit your radio’s memory using CHIRP or any spreadsheet editor.


📦 Included Scripts
1. ChirpCSV_to_YSF.py

Converts a CHIRP-exported CSV into a valid .YSF file ready to upload into the Hiroyasu IC-980Pro.

The full pipeline is automatic:

CHIRP CSV → Hiroyasu-formatted CSV → YSF codeplug


Output:

YSF_<original_name>.ysf

2. HiroyasuYSF_to_ChirpCSV.py

Extracts all channels from a Hiroyasu .YSF file and converts them into a clean, CHIRP-compatible CSV.

Useful for:

Editing an existing codeplug

Fixing or cleaning corrupted memories

Migrating from the official CPS to CHIRP workflow

Output:

CHIRP_CSV_<filename>.csv


🧰 Requirements

Python 3.7+

Works on Windows, Linux, macOS

No external libraries required


🚀 How to Use
A) Convert CHIRP CSV → YSF

Export your channel list from CHIRP as CSV

Drag & drop the CSV file onto:

ChirpCSV_to_YSF.py



The script will automatically:

Validate required scripts

Convert the CSV to Hiroyasu format

Encode the .YSF file

Your finished file will appear as:

YSF_<filename>.ysf


Upload this .YSF into your radio using the official Hiroyasu CPS.


B) Convert YSF → CHIRP CSV

Take any .YSF file from the radio

Drag & drop it onto:

HiroyasuYSF_to_ChirpCSV.py


The script will:

Decode the binary YSF structure

Extract all channels

Normalize tones, bandwidth, flags

Produce a clean CHIRP-style CSV

Output file:

CHIRP_CSV_<filename>.csv


Open this CSV in CHIRP or Excel, edit freely, and convert back to YSF when ready.


⚠️ Notes & Recommendations

Always use CHIRP’s UV-5R/UV17-R or similar template before converting (guarantees stable export structure).

The scripts fully support:

CTCSS

DCS

Cross-mode

Split frequencies

Scan / busy lockout flags

Scramble

Channels with missing data are safely cleaned or ignored.

🎥 Instruction Video

https://youtu.be/0VDHweB8ccU

73 de LU7CGJ – Guido Camji

Enjoy the first fully working CHIRP ↔ Hiroyasu workflow available anywhere.
--------------------------------------------------------
SEO Keywords (for indexing and search engines)

CHIRP Hiroyasu IC-980Pro
CHIRP compatibility Hiroyasu
IC-980Pro CSV YSF converter CHIRP
Hiroyasu IC-980Pro programming CPS YSF decoder encoder
