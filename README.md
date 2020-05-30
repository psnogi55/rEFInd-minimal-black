## Minimalistic black rEFInd theme with VISIBLE FONTS

[rEFInd](http://www.rodsbooks.com/refind/) is a simplistic boot manager for UEFI
based systems. This is a clean and minimal black theme for it WITH FONTS.


## Method

Step 1: Download rEFInd

	https://sourceforge.net/projects/refind/

Step 2: Watch the video below
		
	https://www.youtube.com/watch?v=eQXdxTva1WA

Step 3: Themes folder copy

Usage

1.	Locate your refind EFI directory. This is commonly /boot/EFI/refind though it will depend on where you mount your ESP and where rEFInd is installed. See Step 4 : Part 2 for same.
2.	Create a folder called themes inside it, if it doesn't already exist
3.	Clone this repository into the themes directory.
4.	To enable the theme add include themes/black/theme.conf at the end of refind.conf.
Entries that are autodetected should also show the proper icons.
Attribution
The OS icons are from Lightness for burg by SWOriginal.

Step 4: Additional Items

Part 1: Disabling SIP 

How to turn off System Integrity Protection in macOS
		Click the Apple symbol in the Menu bar.
		Click Restart…
		Hold down Command-R to reboot into Recovery Mode.
		Click Utilities.
		Select Terminal.
		Type csrutil disable.
		Press Return or Enter on your keyboard.
		Click the Apple symbol in the Menu bar.
		Click Restart…

Please Enable with “csrutil enable” after completion.


Part 2: Mounting commands

sudo mkdir /Volumes/efi

sudo mount -t msdos /dev/disk0s1 /Volumes/efi


Part 3: What if rEFInd crashes and no black screen on loading mac – Resetting PRAM

(Credits: Applegazette)

Do PRMS Reset - The Mac’s PRAM is memory that holds some settings for your Mac. These settings carry forward even if you restart or shut down the Mac. If they get corrupted somehow, it can cause problems like a black screen.

To reset the PRAM, power on your Mac and as soon as you hear the startup chime, hold the Command+Option+P+R keys. Wait until you hear the chime a second time and then let go of the keys. Let the Mac boot and see if the black screen is fixed.
