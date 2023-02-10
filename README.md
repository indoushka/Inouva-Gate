Author: <b><i>indoushka</i></b><br />
Version release: <b><i>v2.10.13</i></b><br />
Distros Supported: <b><i>Windows (x86|x64), Linux</i></b><br />
Inspired in the work of: ['@r00t-3xp10it - meterpeter']([https://github.com/ZHacker13/ReverseTCPShell](https://github.com/r00t-3xp10it/meterpeter/))<br /><br />

## :octocat: Project Description
This PS1 starts a listener Server on a Windows|Linux attacker machine and generates oneliner PS reverse shell payloads obfuscated in BXOR with a random secret key and another layer of Characters/Variables Obfuscation to be executed on the victim machine (The payload will also execute AMSI reflection bypass in current session to evade AMSI detection while working). You can also recive the generated oneliner reverse shell connection via netcat. (in this case you will lose the C2 functionalities like screenshot, upload, download files, Keylogger, AdvInfo, PostExploit, etc)<br /><br />meterpeter payloads/droppers can be executed using User or Administrator Privileges depending of the cenario (executing the Client as Administrator will unlock ALL Server Modules, amsi bypasses, etc.). Droppers mimic a fake KB Security Update while in background download\exec Client in '<b><i>$Env:TMP</i></b>' trusted location, with the intent of evading  Windows Defender Exploit Guard. meterpeter payloads|droppers are FUD (please dont test samples on VirusTotal).<br />

Under Linux users required to install **powershell** and **apache2** webserver, Under Windows its optional the install of **python3** http.server to deliver payloads under LAN networks. If this requirements are **NOT** met, then the Client ( <b><i>Update-KB4524147.ps1</i></b> ) will be written in meterpeter working directory for manual deliver.
