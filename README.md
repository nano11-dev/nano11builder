# Nano11Builder

A script to make your OWN Nano11 image.

This is a script to automate the build of an Nano 11 iso.
The main goal of this is to use only Microsoft utilities like DISM, and nothing external. The only executable included is oscdimg.exe, which is provided in the Windows ADK and it is used to create bootable ISO images. Also included is an unattended answer file, which is used to bypass the MS account on OOBE.

To download the post-setup, you will need git If you don't want to install it, you can skip the step

Instructions:

1. Download an Windows 11 ISO.
2. Mount the downloaded ISO image using Windows Explorer.
3. Run the nano11builder.bat file.
4. Select the drive letter where the image is mounted (only the letter, no colon (:))
5. Select the SKU that you want the image to be based.
6. Sit back and relax :)
7. When the image is completed, you will see it in the folder where the script was extracted, with the name nano11.iso

What is removed:

Everything Nano11 Removes

Known issues:

1. Only en-us x64 is supported as of now. This can be easily fixable by the end user, just by replacing every instance of en-us with the language needed (like ro-RO and so on), and every x64 instance with arm64.

And that's pretty much it for now!
