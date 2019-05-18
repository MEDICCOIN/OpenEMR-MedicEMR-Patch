# MedicEMR

MedicEMR is a powerful OpenEMR with [Medic Coin](https://mediccoin.com) blockchain as a form of payment.

MedicEMR is a fork of OpenEMR and is the most popular open source electronic health records and medical practice management solution. ONC certified with international usage, MedicEMR's goal is a superior alternative to its proprietary counterparts.

## Open Source MedicEMR

Open Source MedicEMR is always available to download at https://github.com/MEDICCOIN/Medic-EMR/releases/latest

## Hosted MedicEMR

You can start your MedicEMR site instantly at https://medicemr.com. It's free and mantained by the MedicCoin Support Team.

# OpenEMR to MedicEMR Patch

If you already use OpenEMR but want to accept Medic Coin as a form of payment, you just need to patch your OpenEMR to turn it to MedicEMR.

## OpenEMR 5.0.1.x to MedicEMR 5.0.1.x

* First of all, generate a backup of your OpenEMR: databases, files. Consult your hosting documents to know how to backup your OpenEMR.
* Change current directory to root of your OpenEMR:
```sh
cd /Path/to/OpenEMR
```
Replace `/Path/to/OpenEMR` with path to root of your OpenEMR where contains folders like apis, ccr, gacl, portal, version.php
* If your OpenEMR is from v5.0.1.4 to v5.0.1.6:
```sh
curl -s https://raw.githubusercontent.com/MEDICCOIN/OpenEMR-MedicEMR-Patch/master/openemr-v5.0.1-medicemr-v5.0.1.patch | patch -p2
```
* If your OpenEMR is from v5.0.1.7 or higher:
```sh
curl -s https://raw.githubusercontent.com/MEDICCOIN/OpenEMR-MedicEMR-Patch/master/openemr-v5.0.1.7-medicemr-v5.0.1.7.patch | patch -p2
```
