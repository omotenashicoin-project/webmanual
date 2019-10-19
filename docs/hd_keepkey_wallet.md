# HARDWARE WALLET CLIENT FOR KEEPKEY GUIDE

## TARGET AUDIENCE
This guide is for users who use a Keepkey hardware wallet with Electrum-MTNS wallet.

## OUTLINE
Install the OmotenashiCoin firmware for keepkey in your hardware wallet in advance.  
When updating the firmware, transfer the crypto assets in the hardware wallet to another wallet.  
Click here for details on [installing keepkey firmware](http://users-manual.org/hardware_firmware_keepkey/ "installing keepkey firmware").  
This page mainly describes how to use the Keepkey device.

## INITIAL SETTING
This section describes the configuration steps immediately after installing the MTNS keepkey firmware.  

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
connect Keepkey device on your PC.
![Screenshot](img/DSC01902.JPG)

1. Select Auto connect.  
![Screenshot](img/ele_17-04.png)  
2. Input your wallet name.  
A wallet file is created with the name entered here.  
This is the name that is referred when managing multiple wallets with one Electrom-MTNS.  
![Screenshot](img/ele_17-44.png)
3. Select Stantard wallet.  
![Screenshot](img/ele_17-55.png)
4. Select Use a hardware device.  
![Screenshot](img/ele_18-12.png)
5. This appears when a Keepekey device is found.  
If the screen is different and you are using Windows, [please refer to this page](http://users-manual.org/hd_client_wallet/#about-the-general "please refer to this page").
![Screenshot](img/ele_04-55.jpg)
6. Initialize setting
Click Next button.  
![Screenshot](img/elein_52-50.png)  
Click Next button.  
If you want to use more words, select 24words.
![Screenshot](img/elein_53-21.png)   
7. set PIN code and get seed charactors.  
go to your keepkey device.  
If you press and hold the button on the keepkey body,  
the [▲] image on the screen changes to [ ﾚ ] and the screen moves to the next screen.  
![Screenshot](img/DSC01903.JPG)
![Screenshot](img/DSC01904.JPG)  
go to Electrum-MTNS on your PC   
Map the display contents of the device and the area displayed by Electrum,   
click the button of the corresponding location, and register the PIN code.  
ex) if you want to input 1 and 5, The mapping with 1, 5 is like this.  
![Screenshot](img/elein_78-44.jpg)  
![Screenshot](img/elein_55-20.png)  
go to your keepkey device.  
press and hold the button on the keepkey body.  
![Screenshot](img/DSC01905.JPG)
![Screenshot](img/DSC01906.JPG)
8. Select legacy.
Omotenashicoin supports only p2pkh.
Other addresses type are not supported.
![Screenshot](img/ele_18-40.png)
9. Finally, select whether to encrypt the wallet from the checkbox.
![Screenshot](img/ele_18-52.png)

## HOW TO TRANSFER MTNS ASSETS
This section describes the procedure for transferring MTNS.
This asset transfer is a state where the MTNS asset already exists in the hardware wallet.

### transferring MTNS other address
1. Open the Electrum-MTNS wallet, and send tab clicked.  
Input Pay to address and amount, then click Send button.  
Perform the procedure while checking your Electrum-MTNS and Keepkey Device.  
![Screenshot](img/elesend_06-46.png)  
![Screenshot](img/elesend_00-46.png)  
![Screenshot](img/elesend_01-15.png)  
If you press and hold the button on the keepkey body,   
the [▲] image on the screen changes to [ ﾚ ] and the screen moves to the next screen.  
![Screenshot](img/DSC01907.JPG)  
your PC  
![Screenshot](img/elesend_01-40.png)  
press and hold the button on the keepkey body.  
![Screenshot](img/DSC01908.JPG)  
your PC  
![Screenshot](img/elesend_01-48.png)  
press and hold the button on the keepkey body.  
![Screenshot](img/DSC01909.JPG)  
your PC  
![Screenshot](img/elesend_02-15.png)  

Transferring MTNS success.

