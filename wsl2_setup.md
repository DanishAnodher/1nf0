# WSL2 Setup (Windows Subsystem for Linux)
---

## About
Windows Subsystem for Linux (WSL) is a feature of Windows that allows developers to run a Linux environment without the need for a separate virtual machine or dual booting.

## Requirements
* WSL 2 requires Windows 11,[57] or Windows 10 version 1903 or higher, with Build 18362 or higher, for x64 systems, and Version 2004 or higher, with Build 19041 or higher, for ARM64 systems.

## Steps

* Open Windows `Powershell` as administrator

* Paste and Run the following commands
```
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
* `Restart` your PC / Laptop

* Now paste the following command in the `powershell`
```
wsl --set-default-version 2
```
* Lastly, Install any linux distribution from the `Microsoft Store`:
  * [Kali Linux](https://apps.microsoft.com/store/detail/kali-linux/9PKR34TNCV07?hl=en-pk&gl=pk&ref=hackernoon.com&rtc=1)
  * [Ubuntu](https://apps.microsoft.com/store/detail/ubuntu/9PDXGNCFSCZV)


Run the installed distro from `start-up`, wait untill it's installed and you're good to go.
