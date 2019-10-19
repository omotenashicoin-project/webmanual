# HOW TO INSTALL LEDGER WALLET FIRMWARE

<font color="red">
Now being created
</font>




## OUTLINE
This page is a guideline for installing OmotenashiCoin firmware on Ledger hardware devices.  
Ledger device can be used as a wallet of OmotenashiCoin by installing MTNS firmware according to the following procedure.  
As of February 2020, Ledger does not yet officially support OmotenashiCoin.  
If you want to install custom firmware, see this page.  
It's a little complicated to update Ledger firmware.  
After installing the compiler to compile the firmware, build and update the Ledger device.  

This step is not necessary after Ledger has officially supported OmotenashiCoin.  
These update environments are performed on **Ubuntu 18.04 for Ledger nano s with bootloader version 1.8.0**.  
**We have not confirmed the operation of other Ledger devices .**  
## IMPORTANT INFOMATIONS
<span style="color: red; ">
If you already have other coin funds in your LEDGER wallet,  
be sure TO TRANSFER THE FUNDS TO ANOTHER WALLET.  
Please use only those who have accepted the [terms of use / disclaimer](http://users-manual.org/disclaimer/ "terms of use / disclaimer").
</span>


## DOWNLOAD LEDGER BUILD TOOLS

## SETUP YOUR ENVS

## INSTALL MTNS FIRMWARE TO LEDGER WALLET

### Download MTNS firmware for a ledger device from our github web url.
```
$ git clone https://github.com/omotenashicoin-project/ledger-app-btc.git
$ ls ledger-app-btc
```

### Install custom MTNS  ledger firmware
1. Connecting USB cable while holding down the 2 buttons (right and left buttons simultaneously) of the Ledger.  
The boot loader screen will be displayed.
display message: 
![Screenshot](DSC01927.JPG)

2. Enter ledgerctl command.  
` $ ledgerctl firmware-update -f ledger.bin`
> After executing the command, the following information is displayed on the command line.  
> Enter "y" in the "No signatures found. Continue? [Y / N]" line and enter.  
>> Ledger One v2 firmware (1.8.0 or later)  
Firmware version 1.9.0 build 0  
**No signatures found. Continue? [y/N]: y**  
Unsigned firmware looking OK.  
Firmware fingerprint: e35809b5521789a281481d10897a4ab837b9aa802c0a54c0f52b1c19aaebe6bd  
Please confirm action on your Ledger device  
Please confirm action on your Ledger device    
3. Go back your ledger device.  
Push the right button on the ledger body.  
![Screenshot](DSC01928.JPG)  
Push right button. will be started firmware instration. 
![Screenshot](DSC01929.JPG)
![Screenshot](DSC01930.JPG)
Push the right button on the ledger body.  
![Screenshot](DSC01931.JPG)
![Screenshot](DSC01932.JPG)
4. Disconnect usb cable from your ledger device, then reconnect.
5. A warning is displayed for custom firmware.
Push the right button.   
![Screenshot](DSC01933.JPG)
Push the right button.   
![Screenshot](DSC01934.JPG)
After a while, the following screen is displayed.  
![Screenshot](DSC01935.JPG)

MTNS firmware install success.

To use Ledger now, go to this URL
[Hardware Wallet (Ledger))](http://users-manual.org/hd_ledger_wallet/ "Hardware Wallet (Ledger))")




