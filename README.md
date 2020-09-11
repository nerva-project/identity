# NERVA Identities

This repo contains the public key for Nerva developer Angry Wasp, used to sign the NERVA 0.1.7.1 CLI and 2.8.0 GUI binaries.

The following download links provide binaries signed with this key

## Valid CLI Links

### Linux

Binary: [https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_linux.zip](https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_linux.zip)  
Sig:    [https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_linux.zip.sig](https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_linux.zip.sig)

### OSX

Binary: [https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_osx.zip](https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_osx.zip)  
Sig:    [https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_osx.zip.sig](https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_osx.zip.sig)  

### Windows

Binary: [https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_windows.zip](https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_windows.zip)  
Sig:    [https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_windows.zip.sig](https://bitbucket.org/nerva-xnv/nerva/downloads/nerva-v0.1.7.1_windows.zip.sig)  

## Valid GUI Links

### Linux

Binary: [https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_linux.zip](https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_linux.zip)  
Sig:    [https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_linux.zip.sig](https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_linux.zip.sig)

### OSX

Binary: [https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_osx.zip](https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_osx.zip)  
Sig:    [https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_osx.zip.sig](https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_osx.zip.sig)  

### Windows

Binary: [https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_windows.zip.zip](https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_windows.zip)  
Sig:    [https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_windows.zip.sig](https://bitbucket.org/nerva-xnv/gui/downloads/nerva-gui-v2.8.0_windows.zip.sig) 


Binaries should only be downloaded from the above links and verified against the public key listed in this repo with the provided detached signature files

## Verifying File Integrity

Download the `AngryWasp.asc` file in this repo  
Import the key with `gpg --import AngryWasp.asc`  
Verify the imported key `gpg --fingerprint angrywasp`  

The result should show a key with a public key fingerprint of  
`B743 742C 766C 93DA 80D7  7B75 B987 8FFD A039 B5A4`  
and a uid of  
`Angry Wasp <angrywasp@live.com>`

If these details are correct, you can verify the binary by downloading the binary and detached signature file to the same directory and using the command  
`gpg --verify <file>.zip.sig`  
GPG will report back  
`Good signature from "Angry Wasp <angrywasp@live.com>"`

If the key has been verified and the binary reports the signature is good, it is safe to extract and use this software. if any part of this process fails or returns unexpected results, the binary and public key file should be discarded. It is always recommended to build from source.