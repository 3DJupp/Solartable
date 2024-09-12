# Solartable
Project that will utilize a solar panel and some aluminum profiles as an outdoor / garden table
![SolarTable-1](https://user-images.githubusercontent.com/8407566/233850090-255ac83c-c0e9-4d08-bece-515f9f898cc9.jpg)
As I am based in Germany, I might take care of the regulations that apply here. (more in the preface)

## Preface
For a long time, I wanted to have a small photovoltaic system to reduce energy costs and produce a portion of my household electricity on my own. There have been and are a lot of regulations in Germany. Thus, there is a European law that should permit the installation of small solar panels and microinverters there are still a lot of more or less useful regulations. A table is a way of having a hassle-free "balcony power station". So at some point, my local public utilities company changed their laws and switched my electricity meter to a bidirectional one. I have still not heard anything by the landlord, but as a permit for a table is not required, I was able to start the project.

## Build process
At some day, I was finally able to pick up the modules at a local Solar Systems builder. At first, I wanted to build that frame utilizing wood, but for some reason I thought black aluminum profiles are more durable.

### Assembly
I chose the panel "ASWS Strong Style 390-MH120-N 390 Watt" and had a look in the [datasheet](https://shop.erene.de/media/14/16/0c/1679044263/datenblatt-ASWS-390-MH120N-BG-deutsch.pdf) for the dimensions.
So I wrote down the numbers and calculated how many aluminum bars were required.
I came down to this Bill of materials. I used to order at the shop "myaluprofil" - but they are too expensive nowadays please search for the 3030 profiles, you'll find tons of shops

|Count|Article|Article-Nr.|Price per unit|Total|Length|
|-----|---------------------------------------------------|----------------|--------------|-------|-------|
|8 x|Winkelsatz 30x30 schwarz Nut 6 I-Typ|xxx|3,20 EUR|25,60 EUR||
|4 x|Kreuz-Kabelbinderblock Nut 6 I-Raster PA|xxx|0,95 EUR|3,80 EUR||
|8 x|Winkelsatz 30x60 ZN Nut 6 I-Typ|xxx|5,80 EUR|46,40 EUR||
|4 x|Nutenstein mit Steg Nut 6 I-Typ M6|xxx|0,35 EUR|1,40 EUR||
|4 x|Aluminiumprofil 30x30 Nut 6 I-Typ Leicht 1N Schwarz|xxx|12,25 EUR|49,00 EUR|**700 mm**|
|2 x|Aluminiumprofil 30x30 Nut 6 I-Typ Leicht 2N90 Schwarz|xxx|16,40 EUR|32,80 EUR|**975 mm**|
|1 x|Aluminiumprofil 30x60 Nut 6 I-Typ Schwarz|xxx|30,06 EUR|30,06 EUR|**1400 mm**|

The legs will be attached using a large angle (30 by 60 mm) on the two crossbars and on the panel (the frame itself) using two smaller (30 by 30 mm) angles, which are in black the same color as the frame. The crossbars will be attached on the large 30x60 aluminum rod using two of the gray angles. For stability reasons, you could also use the large angles (30 by 60 mm), but that depends on your budget.

I mounted the frame itself, placed the solar panel facing upside down, mounted the small angles on the legs. Finally, I was able to mark the spots where I will drill some holes. Please use a spare wood part or anything else, as you should not hit the panel/glass surface with the drill bit.
![SolarTable-2](https://user-images.githubusercontent.com/8407566/233850363-1c598d4a-3f2b-4b11-a18a-b6c80714d090.jpg)
The frame is placed on top of the solar panel, placed upside-down on a blanket.

After that I rotated the frame for mounting the inverter, which was mounted using two sliding blocks, washers and M6 screws on the large 30x60mm profile.
![SolarTable-3](https://user-images.githubusercontent.com/8407566/233850353-11011db4-9abf-4294-8065-587846ed7408.jpg)

### Electrical installation

As we are dealing with a solar panel, that's meant to produce electricity we want to be able to make use of.
**I would suggest to work with electricity only if you are familiar with it. No matter if it's AC, DC - 30 or 240 Volts. Otherwise, please consult an electrician.**

As I was not happy with the connectors and safety measurements that come with some microinverters, I built the unit as follows.:
- I found some connectors that are certified to be waterproof and also hot-plug-capable.
  Normally, these kinds of connectors are widely known in event technology, but why shouldn't I use them in my project? Thanks to [Neutrik](https://www.neutrik.com) for their great piece of engineering.
- Secondly, I wanted to have a dedicated RCD and circuit breaker. This is meant to reduce the risk of overloads (breaker) and electrocution (RCD, or "Residual Current   Device", in Germany also known as "FI"). The combination of RCD and circuit breaker is known as "FI/LS" in Germany.

When working with proper tools, the installation of solar panels or electric components in general is easier and more reliable.
Personally i use tools from [Knipex](https://www.knipex.com) like this special plier for solar or thicker outdoor-cables:
![SolarTable-4](https://user-images.githubusercontent.com/8407566/233867078-e29ea0e3-dcef-42c3-b98c-d19d2915f5b4.jpg)
So as mentioned, i wanted to get rid of the connectors that came with the inverter I got from "Hoymiles", after unscrewing the connector, i was able to see three wires. Red, Black and Green/Yellow. ![SolarTable-5](https://user-images.githubusercontent.com/8407566/233867175-01b903f1-f752-464b-bcce-7af2eb055465.jpg)
- Green/Yellow means Earth/Protective wire. (As it should be all around the world)
- Red means "Hot" or "Live wire", so thats where the "240 V AC" should be applied.
- Black means neutral, same potential as "Earth" but thats the return for a load or generator in our case.

I also suggest so add ferrules to the end of those wires, like I already did in that pictures. Typically those wires were soldered together with a small amount of tin/lead.
So at first, i will provide you this close-up of the crowded junction box I made and will explain whats going on here.
![SolarTable-6](https://user-images.githubusercontent.com/8407566/233868076-9502e440-a460-40cd-b1fa-b916dd87ef23.jpg)
The big unit labeled by the company "Schneider Electric" is our combined RCD/Breaker. It's rated to 6 Ampere for the CB specs and 30mA for the RCD specs. Talking about the CB: 6 Amps is less than the outlets and connectors are rated to. (Approximately 230V*6A=1380VA/W / not too accurate as we are dealing with alternating current), in any case, this breaker should trip before the "normal" ones we can typically found in our houses will do. (The outlets and breakers are typically rated to 16 Amps/~3.680 Watts)
Another thing about having a second RCD in series: Not all households have RCDs installed, yet they have to at a certain point. So in case there is a "leak" of current from the live wire, the RCD will detect it and trip (it will also shut down the circuit breaker)
I used two outlets from Neutrik, the Powercon True1 TOP series, one is the input, and the other one is the output.
The input is connected to the RCD/CB and the output is connected to the Powercon Outlet on the other side, to our inverter etc.
The earth wire is always connected between input, output and any other metal part, like the DIN-Rail. It should not be interupted.

**I will add a part list from Reichelt here:**
|Count|Article|Article-Nr.|Price per unit|Total|Comment|
|-----|---------------------------------------------------|----------------|--------------|-------|-------|
|1 x|Verteilerkasten Feuchtraum, 1-reihig, 4 Module|DB-F 1-4 TR|28,20 EUR|28,20 EUR|Junction-Box|
|1 x|powerCON TRUE1 TOP Gerätestecker, Inlet|PCON MPX-TOP|3,90 EUR|3,90 EUR|Power In (Socket)|
|1 x|powerCON TRUE1 TOP Kabelbuchse, Outlet|PCON FX-W-TOP|9,05 EUR|9,05 EUR|Power Out (Plug to connect to MPX-TOP)|
|1 x|powerCON TRUE1 TOP Geräteeinbaubuchse, Outlet|PCON FPX-TOP|6,99 EUR|6,99 EUR|Power Out (Socket, optional)|
|1 x|powerCON TRUE1 TOP Kabelbuchse|PCON MX-W-TOP|8,99 EUR|8,99 EUR|Power In (Plug to connect to FPX-TOP)|
|1 x|Betteri BC01, Buchse (female), AC 3-polig, IP67|BETTERI BC01F|12,99 EUR|12,99 EUR|If you prefer the Betteri-connector instead of Neutrik|
|1 x|Betteri BC01, Endkappe (für female), AC 3-polig, IP67|BETTERI BC01FK|7,99 EUR|7,99 EUR|If needed, cap for the inverter output|
|1 x|FI/LS-Schalter Resi9 1P+N, 6A, B-Char., 30mA, Typ A, 6kA|R9D01606|61,95 EUR|61,95 EUR|RCD/CB|

Other connectors might be possible, but i won't add them to the BoM, i also not added ferrules, wires, crimp connectors etc. to not overcomplicate things.
For the DIN-Rail connectors I used the [PTFIX Series/Phoenix Contact](https://www.reichelt.de/verteilerblock-ptfix-12x2-5-blau-ptfix-12x2-5-bu-p262114.html) and [WPE 4/Weidmüller](https://catalog.weidmueller.com/catalog/Start.do?&ObjectID=1010100000) for the PE-Connector. The Betteri Cap and Connector is only needed, when keeping at least one Betteri Plug connected to the Inverter. (I removed ine female/inlet and connected it directly using the PTFIX, as they are 4mm² wires)

When the junction box is wired properly, you can close it (those screws were a bit annoying) and ad a cover, if there is space left:
![PXL_20230501_180927375](https://user-images.githubusercontent.com/8407566/235510978-417d062b-ef50-405b-aeb5-d934f15c9b09.jpg)



## Part list / BoM
I used several parts to build this table. In this project I will utilize aluminum extrusion profiles, which were also widely known in industry usages (CNC, Robotics, 3D-Printers or any other manufacturing process)
This is the part list, including a shop or datasheet for reference. In some cases, I used spare/used parts, so I will link the manufacturer page instead.

I do not get any kind of bonus by mentioning a certain shop. [In case you think that this project is useful, buy me a coffee ☕🫘 instead](https://paypal.me/DSpatz)

|Part|Further information or shop|Price in Euro (€)|
|----|---------------------------|-----------------|
|Solar Panel|[ASWS strong style](https://www.asws-solar.de/solarmodule/strong-style)|€80-€150*|
|Hoymiles Microinverter|[HM 400 Specs](https://www.hoymiles.com/product/microinverter/hm-300-350-400-eu)|€120**|
|Aluminum profiles and accessories|any hardware-store for aluminum profiles|€100-200***|
Cables and electronics like RCD/Circuit Breaker|[reichelt.de](https://www.reichelt.de/)|€10-€150****|

\* I used this module: <ins>ASWS Strong Style 390-MH120-N 390 Watt</ins>, at the time of purchase, I paid around **€250** including VAT (19%) in Germany. There is no need to use a bifacial module, you can definitely go for a cheaper one instead. I think this is more beautiful.

\** I purchased a used module on "[Kleinanzeigen.de](https://kleinanzeigen.de)" / classifieds for around **€115**
 
\*** There might be different vendors of aluminum profiles, thus I don't want to cut them on my own. Unfortunately i can not recommend a certain shop anymore. The one i used before did increse pricing while decreasing service and lead times.

\**** The amount you want to spend here is depending on the functionalities your table should have.
Mine is utilizing a combined circuit breaker and RCD. Shops like "[reichelt.de](https://www.reichelt.de)" should cover your needs. (I also added waterproof connectors, but I explained that in the [section about the electrical installation](#electrical-installation))

### Sources and inspiration from other projects

 - Firstly, thanks to the make-magazine and further resources.
     - [This is the article (paid) from Make 4/2022](https://www.heise.de/select/make/2022/4/2215210171328615510)
 - [solartisch.de / a collection of resources for solar tables](http://solartisch.de)
 - Fablab with the wooden Table:
    - [Hackster.io. article](https://www.hackster.io/fablabeu/solartisch-91a1d8)
    - [TinkerCad / Resources for a wooden table](https://www.tinkercad.com/things/hHsPlie2SS3-solartisch)
 - [solartisch.com and other commercial projects](https://solartisch.com)
