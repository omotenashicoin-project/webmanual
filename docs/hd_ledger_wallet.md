# HARDWARE WALLET CLIENT FOR LEDGER GUIDE
<font color="red">
Now being created
</font>
## TARGET AUDIENCE
This guide is for users who use a Ledger hardware wallet with Electrum-MTNS wallet.

## OUTLINE
Install the OmotenashiCoin firmware for ledger in your hardware wallet in advance.  
When updating the firmware, transfer the crypto assets in the hardware wallet to another wallet.  
Click here for details on [installing ledger firmware](http://users-manual.org/hardware_firmware_ledger/ "installing ledger firmware").  
This page mainly describes how to use the Ledger device.

## INITIAL SETTING
This section describes the configuration steps immediately after installing the MTNS ledger firmware.  

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
1. Connect Ledger device on your PC.
![Screenshot](DSC01935.JPG)
2. Input your wallet name.  
A wallet file is created with the name entered here.  
This is the name that is referred when managing multiple wallets with one Electrom-MTNS.  
![Screenshot](ele_17-44.png)
3. Select Stantard wallet.  
![Screenshot](ele_17-55.png)
4. Select Use a hardware device.  
![Screenshot](ele_18-12.png)
5. This appears when a Ledger device is found.  
If the screen is different and you are using Windows, [please refer to this page](http://users-manual.org/hd_client_wallet/#about-the-general "please refer to this page").
![Screenshot](eletz-09-35.png)
6. Initialize setting
Click Next button.  
![Screenshot](eletz-09-41.png)  
Go to your Ledger device.  
Push the right button on the ledger body.  
![Screenshot](DSC01937.JPG)
Go to Electrum-MTNS.  
![Screenshot](eletz-09-41.png)  
Click Next button.  
If you want to use more words, select 24words.
![Screenshot](eletz-09-51.png)   
7. set PIN code and get seed charactors.  
go to your ledger device.  
![Screenshot](DSC01938.JPG)
go to Electrum-MTNS on your PC   
Map the display contents of the device and the area displayed by Electrum,   
click the button of the corresponding location, and register the PIN code.  
ex) if you want to input 6 and 9, The mapping with 6, 9 is like this.  
![Screenshot](DSC01939_window.JPG)  
go to your ledger device.  
Push the right button on the ledger body.  
These 12 keywords are very important. Keep it in a safe place.  
![Screenshot](DSC01941.JPG)
![Screenshot](DSC01942.JPG)
![Screenshot](DSC01943.JPG)
After displaying the 12 keywords, you need to check the 12 keywords again.  
Press the right button again.  
8. Select legacy.
Omotenashicoin supports only p2pkh.
Other addresses type are not supported.
![Screenshot](ele_18-40.png)
9. Finally, select whether to encrypt the wallet from the checkbox.
![Screenshot](ele_18-52.png)  
Opened top window.
![Screenshot](eletz-13-16.png)

## HOW TO TRANSFER MTNS ASSETS
This section describes the procedure for transferring MTNS.
This asset transfer is a state where the MTNS asset already exists in the hardware wallet.

### transferring MTNS other address
1. Open the Electrum-MTNS wallet, and send tab clicked.  
Input Pay to address and amount, then click Send button.  
Perform the procedure while checking your Electrum-MTNS and Ledger Device.  
![Screenshot](eletz-23-25.png)  
Push the right button on the ledger.  
The screen will display the amount you have entered.  
![Screenshot](DSC01944.JPG)  
your PC wallet.  
![Screenshot](eletz-20-38.png)  
Push the right button on the ledger.  
The fee is displayed on the screen.  
![Screenshot](DSC01945.JPG)  
your PC wallet.  
![Screenshot](eletz-22-59.png)  
Push the right button on the ledger.  
The screen will show the total amount and fee entered.  
![Screenshot](DSC01947.JPG)  
your PC wallet.  
![Screenshot](eletz-23-10.png)  
  
Transferring MTNS success.

