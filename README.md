# QR Code Faktur Pajak Scanner

A Python application for scanning and processing Indonesian tax invoices (Faktur Pajak) from QR codes. The tool extracts XML data from e-Faktur QR codes, parses the information, and stores it in an Excel file.

## Features

- 🖥️ Real-time QR code scanning using webcam
- 📄 XML data extraction from DJP e-Faktur QR codes
- 🔍 Automatic parsing of tax invoice information including:
  - Seller and buyer details (NPWP, name, address)
  - Invoice number and date
  - Transaction amounts (DPP, PPN, PPnBM)
  - Item details (name, quantity, price)
- 💾 Automatic Excel file generation (`faktur_pembelian.xlsx`)
- 🔊 Audio confirmation on successful scan
- 🔄 Duplicate invoice detection
- 🕒 Timestamp recording for each scan

## Requirements

- Python 3.7+
- Required packages:
  ```bash
  pip install opencv-python pandas numpy sounddevice pyzbar requests openpyxl
