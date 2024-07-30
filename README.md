# SETUP-Pak

Setup Pak and installation guide for setting up Pretendo on Citra.


# Notice
you need a modded 3ds first if you dont have one go to https://3ds.hacks.guide


## Installation

Go download the latest release setup pak and extract it. go into the 3ds folder and copy the files to where they need to go (so the cia files in /cias and 3dsx files in /3ds)

Launch 3ds recovery tool and dump lfcs_b/a, secureinfo_a/b, and aes_keys.txt

Launch ctcert dumper from homebrew launcher it should dump it on the root of the sd.

Then you will want to download Pablomk7's citra: https://github.com/PabloMK7/citra/releases

go into the emulation settings and select those files you dumped (lfcs_b/a, secureinfo_a/b, and ctcert)

And in the main citra root folder, copy the aes_keys.txt into the sysdata folder then download the Home menu

Go extract the load folder into the main citra root folder where all the other folders are

Go to emulation --> debugging --> lle modules then toggle the following: HTTP    NIM     SSL    FRD    BOSS    ACT.

On Android you have to edit CITRA_FOLDER/config/config.ini
where CITRA_FOLDER is the Citra user folder you have set and add the following in the last section (WebService):
```
LLE\HTTP = true
LLE\NIM = true
LLE\SSL = true
LLE\FRD = true
LLE\BOSS = true
LLE\ACT = true
```
There is an example in the config.ini in this repository

Now you can boot the home menu and launch nimbus and select pretendo and it should work (if it crashes then launch the home menu again and you will now be on pretendo)

(To boot home menu: File --> Boot Home menu --> (select region here)

