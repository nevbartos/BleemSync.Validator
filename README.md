# BleemSync validator

## About
A simple utility for verifying that the contents of a USB drive fits the requirements to be able to successfully run [BleemSync]([http://github.com/pathartl/BleemSync) on your PlayStation Classic.

It will perform the following checks:

1. The format of the USB key.
1. The name of USB key is SONY.
1. The required Bleem files and folders are present.
1. Each game folder gets checked for:
    * .bin(s), .cue(s) and .png files are present.
   * Game.ini and pcsx.ini files are present.
   * Each .bin file has a matching .cue file.
   * .bin files have no ',' or '.' in the name.
   * Each .cue file contains the name of the matching.bin file.
   * Game.ini file Discs line contains the name of each .cue file.

## Installation / Usage
Download the ZIP file from the [release](https://github.com/nevbartos/BleemSync.Validator/releases) page.

Extract the contents, create your BleemSync USB key as per the instructions on the BleemSync repo.

Run this utility after your drive is configured, if more than one drive is found, then type the letter of the drive you want to check.

The program will output the name of the check being performed and the status of the check.  

Please note that there are some incompatibilities with newer / USB drives and the PlayStation Classic so even if all the checks pass, it does not mean that your drive will work.

## Notes
Only currently tested on a Windows 10 PC. Please report any problems with other platforms.

This tool will be made obsolete when the UI version of BleemSyns is released.
