# Adobe_Bridge_Show_Geo_Location

Adobe Bridge CC startup-script.

Adds option to photo context menus in Adobe Bridge CC, to see the photo's geo-position on Google Maps (Opens in the default webbrowser).

You _might_ want/need to experiment with how _cmd_ is defined in the code. Mac users should change line #39 to something like:

`var cmd = "open \"https://www.google.com/maps/search/?api=1&query=" + latResult + "," + lonResult + "\"";`

To install, simply copy [the jsx file](https://github.com/StigNygaard/Adobe_Bridge_Show_Geo_Location/raw/master/ShowOnGoogleMaps.jsx) into Adobe Bridge's _Startup Scripts_ folder. To find this folder's location, open Bridge and choose: Preferences -> Startup Scripts -> Reveal My Startup Scripts.

Tested successfully on Windows 10 with Adobe Bridge CC 2020 (v10.0), Bridge CC 2019 (v9.x) and Bridge CC 2018 (v8.x).

I don't really have any knowledge or prior experience on scripting in Adobe CC, but inspired by an [older script by Paul-Riggott](https://github.com/Paul-Riggott/PS-Scripts/blob/master/Map%20from%20Geotag.jsx) (which ain't working in recent CC versions) and a [discussion in Photoshop Family support](https://feedback.photoshop.com/photoshop_family/topics/_mapping_the_photo_in_bridge), I have been able to create this. Also thanks to @geneparcellano for above mentioned modification for Mac users.
