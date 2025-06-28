# PicoCalc Reverse Engineered Back Case

![overview_green.jpg](/resources/images/overview_green.jpg)

## Contents
- [PicoCalc Reverse Engineered Back Case](#picocalc-reverse-engineered-back-case)
  - [Contents](#contents)
    - [Quick Start Guide 🏃‍➡️](#quick-start-guide-️)
  - [What is this?](#what-is-this)
  - [Why is this? 🐛](#why-is-this-)
  - [Improvements 📈](#improvements-)
  - [Variants 🎨](#variants-)<br>
        - [Model A:](#model-a)<br>
        - [Model B:](#model-b)<br>
        - [Model C:](#model-c)<br>
        - [Model D:](#model-d)<br>
  - [Remarks ⚠️](#remarks-️)<br>
        - [Notes on 3D Printing:](#notes-on-3d-printing)<br>
        - [Example Photos 📷](#example-photos-)<br>
  - [Next Steps👷](#next-steps)
  - [Thanks to, 🙌](#thanks-to-)
  - [License 📜](#license-)
  - [Support My Work ☕](#support-my-work-)

### Quick Start Guide 🏃‍➡️
Want to get going quickly without getting lost in the weeds? 

Or want something you can print today and possibly assemble with hardware you have on hand?

[Click here](#model-d) for a shortcut to the Model D section! 
<br>

## What is this?
A new reverse engineered drop in back design for the [ClockworkPi PicoCalc](https://github.com/clockworkpi/PicoCalc)! 

## Why is this? 🐛
 ClockworkPi generously provides original CAD files, but these are optimized for injection molding, with draft angles and injection-molded features that complicate modification in CAD programs like SolidWorks or OpenSCAD. This also prevents perpendicular surfaces necessary for clean FFF 3D printing. 

To alleviate this I have reverse engineered the back case using my PicoCalc and the .step model from Clockworkpi as a guide. After over 200 grams of test prints, the new case back is tuned as a drop-in replacement.  The SD card, 3.5 TRS jack, volume wheel, etc. all fit with no filing or fighting, the bolt pattern aligning naturally. The standard steel DIN912 M3x8 screws provided with the PicoCalc are also perfectly compatible with this case back. 

## Improvements 📈
![frontal_green_labeled.jpg](/resources/images/frontal_green_labeled.jpg)
All versions of the model incorporate a new support bridge near the center in the area between the keyboard and screen.  This was done to add new hardware mounting points but also improves keyboard feel by giving it support at its top edge vastly improving key to key feel consistency. 

## Variants 🎨
![3_4_rear_labeled_green.jpg](/resources/images/3_4_rear_labeled_green.jpg)
There are a few variants of the model that I have provided in this repository.  They are to serve as a basis for anyone else who would like to build a custom back cover or serve as a drop in replacement if user requirements are met.

##### Model A:
This model is only the first ~5 mm of the case and is meant to serve as a basis for any custom designs.  The back surface is completely flat making it easier to modify than cutting and adding to the OEM .step model. 


##### Model B:
Optimized for the PicoCalc with a Luckfox Lyra.  The case is 3mm deeper and incorporates two antenna ports on the top surface (SMA).  It is a two piece model which requires hardware.  Splitting the back cover and back frame allows for optimized clean printing and easy access at the cost of more hardware. Parts needed are listed in the [BOM](https://github.com/Kelpiscool/picocalc-modular-back/blob/main/resources/BOM_Picocalc_case_back_1b.csv).

A landing feature was also incorporated by the 0.1" header pins for easy mounting of PCB addon cards with an M2 threaded insert for support.

Thee back cover consists of a printed in-place live hinge rated for approximately 50–100 open/close cycles before material fatigue becomes an issue. Held down with M3 thumbscrews for easy access.

##### Model C:
Similar to Model B but with added corner bumpers to improve durability of device against hits.  Also replaces left antenna port with a TA4F style connector cutout for non-compliant but ruggedized USB output when using the Luckfox Lyra.  Model is meant to show extensibility and possibilities with this case back family.

##### Model D:
![Model_D_green_labeled.jpg](/resources/images/Model_D_green_labeled.jpg)

This is a quick to get going model that has been simplified for easy use. No antenna cutouts, no heat set inserts, only self tapping holes (go easy when driving the fasteners home!). 

You will already have the $\color{green}\small{\textsf{green}}$ fasteners but this model still needs an extra 7 M3 fasteners or *5 if you still have the two extra included with the PicoCalc* highlighted in $\color{#F85F11}\small{\textsf{orange}}$.  M3x8 fasteners are recommended however M3x6 will also work with less thread engagement. The $\color{#daa520}\small{\textsf{yellow}}$ M2 fastener is also completely optional and only needed if using a daughter card.

Note: This back like the OEM model does not allow easy access to the inside of the device. The threads will also wear and fail after a few assembly and disassembly cycles but this is a great way to test if this back is right for you! 

Links straight to vendors and models ready for Cura or PrusaSlicer.<br>
[Model D Back link](https://github.com/Kelpiscool/picocalc-modular-back/blob/main/models/stl/Custom_back_v.4_model_D.stl)<br>
[Sunstar vent backplate link](https://github.com/Kelpiscool/picocalc-modular-back/blob/main/models/stl/backplate_v.3_sunstar_vent.stl)<br>
Possible vendors for fasteners depending on location.<br>
[If you're stateside (McMaster-Carr)🗽](https://www.mcmaster.com/91292A112/)<br>
[If you're global (AliExpress) 🌏](https://www.aliexpress.us/item/3256803993220034.html) (choose Size: M3, Length: 8 mm)<br>

## Remarks ⚠️
All parts are offered in either a .step file for easy ingestion into CAD programs and workflows. They are also offered in a .stl file made for direct import into a slicer.

Two models of back plate are also offered, one with a sundial vent reminiscent of Clockwork's name. The other is blank for easy customization. 

Dimensions for daughter card are provided in resources\Daughter_card_dimensions.pdf.

##### Notes on 3D Printing:
All prints and tests were done in PETG on a well trammed Ender 3V2 with slower speeds (30-50 mm/s). .2mm slicing height. PEI textured plate with a 5mm brim.  Ideally printed with widest surface facing the build-plate like a pyramid. This hides all supported surfaces inside the case. 

A key post processing step is sanding the power button lightly on the front case facing surface.  If skipped the power button will bind against the case sandwich when torqued down.  By using a draw filing technique with a narrow strip of emory paper (320 grit) adhered to a tongue depressor, a consistent surface finish can be achieved while removing all interference.  This step is best done before breaking the live hinge free.


##### Example Photos 📷
![4in1_example.jpg](/resources/images/4in1_example.jpg)



##  Next Steps👷
- Document and writeup DS3231 RTC integration with Luckfox Lyra only using Python utilizing a lightweight driver by [owainm713](https://github.com/owainm713/DS3231RTC-Python-Module).  <br>
- Integrating a National Instruments GPIB-USB-HS. <br>
- A scroll wheel? 🛞

## Thanks to, 🙌
ClockworkPi forum users:
hisptoot: for getting the Lyra working on the PicoCalc.
markbirss: For getting Ubuntu 24.04 going on the Lyra.<br>
& to ClockworkPi of course for providing a CAD model to work from not to mention making cool hardware devices!<br>

## License 📜
This project is licensed under the CERN-OHL-P-2.0. See the [LICENSE](LICENSE) file for full terms.<br>
<br>
![IMG_3166_resize.jpg](/resources/images/IMG_3166_resize.jpg)

## Support My Work ☕

This project was created for personal use using Solid Edge Community Edition (non-commercial).  
If you found it helpful and want to say thanks, you're welcome to. 🌿

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nitrosomonas)

Ko-fi tips are completely optional, non-commercial, and appreciated.
<br>
By Kelp 🌿 VI/MMXXV.
