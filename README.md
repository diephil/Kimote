#Kimote [![Build Status](https://travis-ci.org/eftov/Kimote.svg?branch=master)](https://travis-ci.org/eftov/Kimote) ![Platforms](https://img.shields.io/badge/platform-ios%20%7C%20android-lightgrey.svg) ![License](https://img.shields.io/badge/license-LGPL%203-blue.svg)

Featured in the [Kodi Wiki](http://kodi.wiki/view/Kimote) and in the [Ionic Showcase (Archive)](http://showcase.ionicframework.com).

#### For both iOS and Android, Kimote is available to test on the Ionic View app with App ID 0E5A555F

---

Kimote is a multi-platform remote application for [Kodi][], developed by 8 telecommunications students from ENSEIRB-MATMECA, a French Engineering School.

It is available for all platforms supported by the [Apache Cordova][] framework but actually only tested on iOS and Android.

On top of Cordova, it is built with [AngularJS][] and the [Ionic][] framework.

##Installation

First, you need to get Cordova and Ionic, with npm : `npm install -g cordova ionic` or download it from the website.

Clone Kimote with `git clone https://github.com/eftov/Kimote.git`.

####Auto install :

Run the install.sh script :

	./install.sh

####Manual install :

Run the following :

	cd Kimote
	ionic start Kimote blank
	rm -r Kimote/www
	mv Kimote/* .
	rm -r Kimote

Add the platforms you need, for example iOS and Android :

	ionic platform add ios
	ionic platform add android

and other supported platforms if you want.

Build it with `ionic build` or just run it on your device  with `ionic run android` and/or `ionic run ios`.

#####Support for ZeroConf on Android

You need to add the ZeroConf plugin to the app directory : `cordova plugins add https://github.com/vstirbu/ZeroConf` to detect Kodi Media Centers automatically.

##Get Kodi/OpenELEC

###Kodi

Kimote is only compatible with Kodi v15 and +. You can download nightly versions from here : <http://mirrors.kodi.tv/nightlies/>

###OpenELEC

If you want Kodi on your RaspberryPi, [OpenELEC][] is the way to go. Clone it from here : <https://github.com/OpenELEC/OpenELEC.tv/tree/openelec-next> and build it yourself.

Or you can just download our compiled version (11 April 2015) available here : https://www.dropbox.com/s/2n7k1jonscizfl6/OpenELEC-RPi.arm-devel-20150411091720-r20584-g254b69d.img?dl=0

##Licensing

Kimote is licensed under the GNU LGPL, Version 3.0. See LICENSE for full license text.

##Contacts

###Supervisors

- Jean-Rémy Falleri - falleri@labri.fr
- Laurent Réveillère - reveillere@enseirb-matmeca.fr

###Students

- Philippe DIEP - Philippe.Diep@enseirb-matmeca.fr
- Moriba DOUMBIA - Moriba.Doumbia@enseirb-matmeca.fr
- Akram EL FADIL - Akram.El_Fadil@enseirb-matmeca.fr
- Benjamin FOVET - Benjamin.Fovet@enseirb-matmeca.fr
- Maxime GASQUE - Maxime.Gasque@enseirb-matmeca.fr
- Aude PLANCHAMP - Aude.Planchamp@enseirb-matmeca.fr
- Héloïse ROSTAN - Heloise.Rostan@enseirb-matmeca.fr
- Anass SEDDIKI - Anass.Seddiki@enseirb-matmeca.fr


[Kodi]: http://kodi.tv/
[Apache Cordova]: https://cordova.apache.org
[AngularJS]: https://angularjs.org/
[Ionic]: http://ionicframework.com/
[OpenELEC]: http://openelec.tv/
