C3 Patch provide's extensive third-party patching capabilities for organizations looking to expand their coverage of third party patches and assess their endpoint and server environments for out-of-date applications. C3 Patch is a C3 site -- for more information on C3 please see the [C3 Homepage.](http://c3.strawgate.com)

# Patching Capabilities

C3 Patch is a software catalog covering a large variety of commonly used third-party software. Our catalog makes patches and content for ~80 common third-party applications. 

## Content Types

The following content is provided for each supported application:

### Deploy
Install an Application if there are no versions of the application installed on the system. This means a Fixlet for an application will only be relevant if:

1. No versions of the application exist on the system
1. The machine meets any prerequisites
1. The machine has enough free disk space

### Update
Update the Application only if an old version of the application is installed. This means an Update Fixlet for an application will only be relevant if:

1. The application exists on the system
1. The application version is older than the version of the fixlet
1. The machine meets any prerequisites
1. The machine has enough free disk space


### Uninstall
Removes the Application only if it is installed. This means an Uninstall Fixlet for an application will only be relevant if:

1. The application exists on the system

## Design Notes

### Dependencies

Dependencies are added as relevance to Deploy and Update fixlets. This means that if the depencies change between versions of an application an update fixlet may not be relevant even though the device is running an out of date version of the application.

### Free Disk Space

Free Disk Space requirements are added as relevance to Deploy and Update Fixlets. This means a machine without an application will not appear as relevant for an application if it does not have enough free disk space.

## Build Statuses

Build information is displayed next to each application. Please note: due to the way builds are currently being run, a failing build can often have a cascading effect on following builds. This means that a failed build may cause the following builds to fail as well for a short time (typically one day). This *does not* mean that we are publishing failing fixlets but instead just means that the fixlets generated are not passing testing and are also not being published.

### Supported Applications 

| Application (83) | Microsoft Windows (80) | Apple macOS (17)
|--- |--- |---		
| 7-Zip | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/1/badge) | 
| Adium | | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/101/badge)
| Air | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/2/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/86/badge) 
| Audacity | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/3/badge) | 
| Atom | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/84/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/87/badge)
| Blender | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/36/badge) | 
| CCleaner | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/34/badge) | 
| CDBurnerXP (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/74/badge) | 
| CDBurnerXP (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/81/badge) | 
| Citrix Receiver | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/48/badge) | 
| Classic Shell | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/4/badge) | 
| CutePDF (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/63/badge) | 
| Cyberduck | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/89/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/88/badge) | 
| Dell Command \| Configure | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/78/badge) | 
| Dell Command \| Update  | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/80/badge) | 
| Dropbox | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/46/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/95/badge)
| Eclipse | | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/104/badge)
| EMET | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/5/badge) | 
| Evernote | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/6/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/96/badge)
| FileZilla | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/7/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/100/badge)
| Firefox | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/77/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/93/badge)
| Foxit Reader | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/33/badge) | 
| GhostScript | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/55/badge) | 
| GIMP | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/8/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/102/badge)
| GIT | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/40/badge) | 
| Google Chrome (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/83/badge) | 
| Google Chrome (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/82/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/97/badge)
| Google Earth | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/32/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/105/badge)
| Greenshot | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/9/badge) | 
| Handbrake (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/92/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/106/badge)
| HipChat | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/73/badge) | 
| ImgBurn | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/44/badge) | 
| Inkscape | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/10/badge) | 
| InstEDIT | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/47/badge) | 
| IrFanView | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/11/badge) | 
| JAWS (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/76/badge) | 
| JAWS (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/75/badge) | 
| KeePass 2 | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/12/badge) | 
| LibreOffice | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/13/badge) | 
| Malware Bytes Anti-Malware | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/15/badge) | 
| Malware Bytes Anti-Exploit | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/79/badge) | 
| Microsoft Security Essentials (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/91/badge) | 
| Microsoft Security Essentials (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/90/badge) | 
| NotePadPP | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/19/badge) | 
| NSClient++ (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/65/badge) | 
| NSClient++ (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/64/badge) | 
| Open Office | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/39/badge) | 
| Opera | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/53/badge) | 
| Paint.Net | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/67/badge) | 
| PeaZip | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/66/badge) | 
| Pidgin | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/18/badge) | 
| Prezi | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/56/badge) | 
| Putty | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/20/badge) | 
| R | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/21/badge) | 
| RealVNC Server (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/23/badge) | 
| RealVNC Server (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/22/badge) | 
| RealVNC Client (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/61/badge) | 
| RealVNC Client (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/62/badge) | 
| Scratch 2 | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/24/badge) | 
| ShareX | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/45/badge) | 
| Silverlight (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/85/badge) | 
| Silverlight (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/25/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/98/badge)
| Steam | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/68/badge) | 
| Teamviewer | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/27/badge) | 
| TextWrangler | | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/103/badge)
| Thunderbird | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/28/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/94/badge)
| TightVNC Server (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/60/badge) | 
| TightVNC Server (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/59/badge) | 
| TightVNC Client (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/57/badge) | 
| TightVNC Client (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/58/badge) | 
| TortoiseSVN (X64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/43/badge) | 
| TortoiseSVN (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/42/badge) | 
| Visio Viewer 2013 | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/38/badge) | 
| VLC | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/30/badge) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/99/badge)
| VMWare Player 12.x | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/31/badge) | 
| VMWare vSphere Client | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/54/badge) | 
| WinDirStat | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/35/badge) | 
| WinMerge | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/52/badge) | 
| Winrar (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/69/badge) | 
| Winrar (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/70/badge) | 
| WinSCP | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/49/badge) | 
| WinZIP (x64) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/51/badge) | 
| WinZIP (x86) | ![Build Badge](https://bfpatch.visualstudio.com/_apis/public/build/definitions/3c2e3afe-6b59-4214-8bd1-0dfcacf59ef8/50/badge) | 


# Support

If you're having issues with the content feel free to create issues in the [Github Repository for this site](https://github.com/strawgate/C3-Patch) or contact me on the [BigFix forum](https://forum.bigfix.com/users/strawgate).

# Contributing

Feel free to make a pull request with any changes or fixes to the content in this site.
