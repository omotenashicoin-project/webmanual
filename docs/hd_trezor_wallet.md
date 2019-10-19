
# HARDWARE WALLET CLIENT FOR TREZOR GUIDE
## TARGET AUDIENCE
This guide is for users who use a Trezor hardware wallet with Electrum-MTNS wallet.

## OUTLINE
Install the OmotenashiCoin firmware for trezor in your hardware wallet in advance.  
When updating the firmware, transfer the crypto assets in the hardware wallet to another wallet.  
Click here for details on [installing trezor firmware](http://users-manual.org/hardware_firmware_trezor/ "installing trezor firmware").  
This page mainly describes how to use the Trezor device.

## INITIAL SETTING
This section describes the configuration steps immediately after installing the MTNS trezor firmware.  

### Download Electrum-MTNS binary file.
```
$ wget https://github.com/omotenashicoin-project/OmotenashiCoin-HDwalletbinaries/raw/master/stable/electrum-mtns-3.3.9-x86_64.AppImage
$ chmod +x electrum-mtns-3.3.9-x86_64.AppImage
```

### Connect your hardware wallet to your PC.

### To run Electrum-MTNS.
```
$ ./electrum-mtns-3.3.9-x86_64.AppImage
```

### Setup Wizard Initial Settings
1. Connect Trezor device on your PC.
![Screenshot](img/DSC01935.JPG)
2. Input your wallet name.  
A wallet file is created with the name entered here.  
This is the name that is referred when managing multiple wallets with one Electrom-MTNS.  
![Screenshot](img/ele_17-44.png)
3. Select Stantard wallet.  
![Screenshot](img/ele_17-55.png)
4. Select Use a hardware device.  
![Screenshot](img/ele_18-12.png)
5. This appears when a Trezor device is found.  
If the screen is different and you are using Windows, [please refer to this page](http://users-manual.org/hd_client_wallet/#about-the-general "please refer to this page").
![Screenshot](img/eletz-09-35.png)
6. Initialize setting
Click Next button.  
![Screenshot](img/eletz-09-41.png)  
Go to your Trezor device.  
Push the right button on the trezor body.  
![Screenshot](img/DSC01937.JPG)
Go to Electrum-MTNS.  
![Screenshot](img/eletz-09-41.png)  
Click Next button.  
If you want to use more words, select 24words.
![Screenshot](img/eletz-09-51.png)   
7. set PIN code and get seed charactors.  
go to your trezor device.  
![Screenshot](img/DSC01938.JPG)
go to Electrum-MTNS on your PC   
Map the display contents of the device and the area displayed by Electrum,   
click the button of the corresponding location, and register the PIN code.  
ex) if you want to input 6 and 9, The mapping with 6, 9 is like this.  
![Screenshot](img/DSC01939_window.JPG)  
go to your trezor device.  
Push the right button on the trezor body.  
These 12 keywords are very important. Keep it in a safe place.  
![Screenshot](img/DSC01941.JPG)
![Screenshot](img/DSC01942.JPG)
![Screenshot](img/DSC01943.JPG)
After displaying the 12 keywords, you need to check the 12 keywords again.  
Press the right button again.  
8. Select legacy.
Omotenashicoin supports only p2pkh.
Other addresses type are not supported.
![Screenshot](img/ele_18-40.png)
9. Finally, select whether to encrypt the wallet from the checkbox.
![Screenshot](img/ele_18-52.png)  
Opened top window.
![Screenshot](img/eletz-13-16.png)

## HOW TO TRANSFER MTNS ASSETS
This section describes the procedure for transferring MTNS.
This asset transfer is a state where the MTNS asset already exists in the hardware wallet.

### transferring MTNS other address
1. Open the Electrum-MTNS wallet, and send tab clicked.  
Input Pay to address and amount, then click Send button.  
Perform the procedure while checking your Electrum-MTNS and Trezor Device.  
![Screenshot](img/eletz-23-25.png)  
Push the right button on the trezor.  
The screen will display the amount you have entered.  
![Screenshot](img/DSC01944.JPG)  
your PC wallet.  
![Screenshot](img/eletz-20-38.png)  
Push the right button on the trezor.  
The fee is displayed on the screen.  
![Screenshot](img/DSC01945.JPG)  
your PC wallet.  
![Screenshot](img/eletz-22-59.png)  
Push the right button on the trezor.  
The screen will show the total amount and fee entered.  
![Screenshot](img/DSC01947.JPG)  
your PC wallet.  
![Screenshot](img/eletz-23-10.png)  
  
Transferring MTNS success.

