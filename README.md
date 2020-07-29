# Filament-Manager-Barcodes

Add barcode support to Octoprint Filament Manager plugin using its API.

## Installation

This repo extends the [Filament Manager Plugin](https://plugins.octoprint.org/plugins/filamentmanager/) written by malnvenshorn.

### Setup Filament Manager

Install the [Filament Manager Plugin](https://plugins.octoprint.org/plugins/filamentmanager/) using my fork to enable real time updates of spools in the UI. `https://github.com/oschwartz10612/OctoPrint-FilamentManager/archive/master.zip`

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

Copy the service to `/etc/systemd/system/`.
```bash
sudo cp scanner.service /etc/systemd/system/scanner.service
```

Enable the Barcode Scanner service so it runs on reboot.

```bash
sudo systemctl enable scanner.service
```

Plug in your barcode scanner and start scanning!
