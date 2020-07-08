# Filament-Manager-Barcodes

Add barcode support to Octoprint Filament Manager plugin using its API.

## Installation

This repo extends the [Filament Manager Plugin](https://plugins.octoprint.org/plugins/filamentmanager/) written by malnvenshorn.

### Setup Filament Manager

Install the [Filament Manager Plugin](https://plugins.octoprint.org/plugins/filamentmanager/)

Configure a default spool profile. This will be the profile that newly scanner spools default to.

### Setup Daemon

Clone the repository onto the Raspberry Pi.

```bash
git clone https://github.com/oschwartz10612/Filament-Manager-Barcodes.git
```

Open the directory.

```bash
cd Filament-Manager-Barcodes
```

Enable the Barcode Scanner service so it runs on reboot.

```bash
sudo systemctl enable scanner.service
```

Plug in your barcode scanner and start scanning!
