# Reliance
Shell script to install a [Reliance Masternode](http://reliance.one/) on a Linux server running Ubuntu 16.04. Use it on your own risk.
***

## Desktop wallet setup  

1. Open the Reliance Desktop Wallet.
2. Go to MasterNode -> My MasterNode
3. Click on Create and fill in the details:
* Alias: MN1
* Address: VPS_IP:43210 (default port)
4. Go to RECEIVE and select : **MN1**
5. Click on Copy address
6. Send **5000** REL to **MN1**. You need to send all 5000 coins in one single transaction.
7. Go back to MasterNode tab and click on **Get Config**.
8. Copy **masternodepvikey** value.
9. Setup Linux VPS 
10. Check if your 5000 REL transaction to yourself has at least 15 confirmations.
11. Go to **Masternodes** -> **My Master Nodes** tab
12. Unlock your wallet if it is encrypted
13. Select your masternode and click on **Start**
14. Login to your VPS and check your masternode status by running the following command. If you get **Status 9**, it means your masternode is active.
```
Reld masternode status
```
***

## Linux VPS Installation
```
wget -q https://raw.githubusercontent.com/zoldur/Reliance/master/reliance_install.sh
bash reliance_install.sh
```

## Usage:
```
Reld masternode status  
Reld getinfo
```
Also, if you want to check/start/stop **Reliance**, run one of the following commands as **root**:

```
systemctl status Reliance #To check if Reliance service is running  
systemctl start Reliance #To start Reliance service  
systemctl stop Reliance #To stop Reliance service  
systemctl is-enabled Reliance #To check if Reliance service is enabled on boot  
```  
***

## Donations

Any donation is highly appreciated

**REL**: RKGVuPM4ynGVKsFC5qeVAbPgrimsArkKn3  
**BTC**: 3MQLEcHXVvxpmwbB811qiC1c6g21ZKa7Jh  
**ETH**: 0x26B9dDa0616FE0759273D651e77Fe7dd7751E01E  
**LTC**: LNZpK4rCd1JVSB3rGKTAnTkudV9So9zexB  
