# Solartable
Project that will utilize a solar panel and some aluminum profiles as an outdoor / garden table
[[/Images/SolarTable-1.jpg|The table can also be used as such.]]

## Preface
For a long time, I wanted to have a small photovoltaic system to reduce energy costs and produce a portion of my household electricity on my own. There have been and are a lot of regulations in Germany. Thus, there is a European law that should permit the installation of small solar panels and microinverters there are still a lot of more or less useful regulations. A table is a way of having a hassle-free "balcony power station". So at some point, my local public utilities company changed their laws and switched my electricity meter to a bidirectional one. I have still not heard anything by the landlord, but as a permit for a table is not required, I was able to start the project.

## Build process
So, at some day, I was finally able to pick up the modules at a local Solar Systems builder. I chose the panel "ASWS Strong Style 390-MH120-N 390 Watt" and had a look in the [datasheet](https://shop.erene.de/media/14/16/0c/1679044263/datenblatt-ASWS-390-MH120N-BG-deutsch.pdf) for the dimensions. At first, I wanted to build that table utilizing wood, but for some reason I thought black aluminum profiles are more durable.
So I wrote down the numbers and calculated how many aluminum bars were required.
I came down to this Bill of materials (Prices as of March 2023) at the shop "myaluprofil":

|Count|Article|Article-Nr.|Price per unit|Total|Length|
|-----|---------------------------------------------------|----------------|--------------|-------|-------|
|8 x|Winkelsatz 30x30 schwarz Nut 6 I-Typ|H206WS30S|3,20 EUR|25,60 EUR||
|4 x|Kreuz-Kabelbinderblock Nut 6 I-Raster PA|H206KKBPA|0,95 EUR|3,80 EUR||
|4 x|Winkelsatz 30x60 ZN Nut 6 I-Typ|H206WS60|5,80 EUR|23,20 EUR||
|4 x|Winkelsatz 30x30 ZN Nut 6 I-Typ|H206WS30|3,30 EUR|13,20 EUR||
|4 x|Nutenstein mit Steg Nut 6 I-Typ M6|H206NSMS6|0,35 EUR|1,40 EUR||
|4 x|Aluminiumprofil 30x30 Nut 6 I-Typ Leicht 1N Schwarz|H1063030L1NSCH|12,25 EUR|49,00 EUR|**700 mm**|
|2 x|Aluminiumprofil 30x30 Nut 6 I-Typ Leicht 2N90 Schwarz|H1063030L2N90SCH|16,40 EUR|32,80 EUR|**~~978~~ 975 mm**|
|1 x|Aluminiumprofil 30x60 Nut 6 I-Typ Schwarz|H1066030LSCH|30,06 EUR|30,06 EUR|**1400 mm**|

**Edit:** turns out I made a small mistake and the supporting bars (H1063030L2N90SCH)  were a bit too long, so I would suggest ordering it in a length of 975 millimeters instead. (not too bad, but worth mentioning)

The legs will be attached using a large angle (30 by 60 mm/H206WS60) on the two crossbars and on the panel (the frame itself) using two smaller (30 by 30 mm/H206WS30S) angles, which are in black the same color as the frame. The crossbars will be attached on the large 30x60 aluminum rod using two of the gray angles (30 by 30 mm/H206WS30). For stability reasons, you could also use the large angles (H206WS60), but that depends on your budget.

I mounted the frame itself, placed the solar panel facing upside down, mounted the small angles on the legs. Finally, I was able to mark the spots where I will drill some holes. Please use a spare wood part or anything else, as you should not hit the panel/glass surface with the drill bit.
[[/Images/SolarTable-2.jpg|The frame is placed on top of the solar panel, placed upside-down on a blanket.]]

I rotated the frame for mounting the inverter, which I mounted using two sliding blocks, washers and M6 screws on the 30x60mm aluminum profile.
[[/Images/SolarTable-3.jpg|The inverter (HM400) is mounted on top of the 30x60 profile.]]

## Part list / BoM
I used several parts to build this table. In this project I will utilize aluminum extrusion profiles, which were also widely known in industry usages (CNC, Robotics, 3D-Printers or any other manufacturing process)
This is the part list, including a shop or datasheet for reference. In some cases, I used spare/used parts, so I will link the manufacturer page instead.

I do not get any kind of bonus by mentioning a certain shop. [In case you think that this project is useful, buy me a coffee ☕🫘 instead](https://paypal.me/DSpatz)

|Part|Further information or shop|Price in Euro (€)|
|----|---------------------------|-----------------|
|Solar Panel|[ASWS strong style](https://www.asws-solar.de/solarmodule/strong-style)            |150-€250*|
|Hoymiles Microinverter|[HM 400 Specs](https://www.hoymiles.com/product/microinverter/hm-300-350-400-eu)|€120**|
|Aluminum profiles and accessories|[myaluprofil.de](https://www.myaluprofil.de/Aluminiumprofile)|€200***|

\* I used this module:  <ins>ASWS Strong Style 390-MH120-N 390 Watt</ins>, at the time of purchase, I paid around **€250** including VAT (19%) in Germany. There is no need to use a bifacial module, you can definitely go for a cheaper one instead. I think this is more beautiful.

\** I purchased a used module on "[eBay Kleinanzeigen](https://www.ebay-kleinanzeigen.de)" / classifieds for around **€115**
 
\*** There might be other vendors of aluminum profiles, thus I don't want to cut them on my own. The advantage of a shop like "[myaluprofil.de](https://www.myaluprofil.de)" is that they offer accessories for the aluminum profiles as well. A detailed BoM can be found in the build-section.

### Sources and inspiration from other projects
 - Firstly, thanks to the make-magazine and further resources.
    - [This is the article (paid) from Make    4/2022](https://www.heise.de/select/make/2022/4/2215210171328615510)
 - [solartisch.de / a collection of resources for solar tables](http://solartisch.de)
 - Fablab with the wooden Table:
    - [Hackster.io. article](https://www.hackster.io/fablabeu/solartisch-91a1d8)
    - [TinkerCad / Resources for a wooden table](https://www.tinkercad.com/things/hHsPlie2SS3-solartisch)
 - [solartisch.com and other commercial projects](https://solartisch.com)