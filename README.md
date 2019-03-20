# FusionX masternode script

* this script was written for debian 9 series; not interested if it doesnt work elsewhere.
* be prepared to paste your masternode's key when prompted (result of 'masternode genkey' from your windows wallet).

you dont need to clone this script from github to use it, just paste (altogether):

```
wget https://raw.githubusercontent.com/FusionEnergyX/FusionX-MNScript/master/mnscript.sh && bash mnscript.sh
```

# What do I do afterwards?

* Once the script prints finished:
1. Open the debug console of your windows wallet
2. Enter `getaccountaddress mn01` at the prompt
3. Send 10000 FUSION to the address that is printed
4. After 15 confirms, enter `masternode outputs` and note the collateral txid and output number
5. From the tools menu, select 'open masternode configuration file'
6. Create a new line at the bottom and enter details as follows:

```
mn01 ipaddressofvps:24999 masternodekey collateraltxid collateraloutputnum
```

for example:
```
mn01 111.112.113.114:24999 63HaYBVUCYjEMeeH1Y4sBGLALQZE1Yc1K64xiqgX37tGBDQL8Xg 2bcd3c84c84f87eaa86e4e56834c92927a07f9e18718810b92e0d0324456a67c 0
```

7. Close the file, and then close the wallet
8. Reopen the wallet; and check the masternode tab (under 'my masternodes')
9. Wait around 5-10 minutes, right click the masternode and select start.


###### barrystyle 20032019
