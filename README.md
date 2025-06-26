# Picocalc Reverse Engineered Back Case

![overview_green.jpg](/resources/images/overview_green.jpg)

## Contents
- [Picocalc Reverse Engineered Back Case](#picocalc-reverse-engineered-back-case)
  - [Contents](#contents)
  - [What is this?](#what-is-this)
  - [Why is this? 🐛](#why-is-this-)
  - [Improvements 📈](#improvements-)
  - [Variants 🎨](#variants-)
        - [Model A:](#model-a)
        - [Model B:](#model-b)
        - [Model C:](#model-c)
  - [Remarks ⚠️](#remarks-️)
        - [Notes on 3D Printing:](#notes-on-3d-printing)
        - [Example Photos 📷](#example-photos-)
  - [Next Steps👷](#next-steps)
  - [Thanks to, 🙌](#thanks-to-)
  - [License 📜](#license-)
  - [Support My Work ☕](#support-my-work-)

## What is this?
A new reverse engineered drop in back design for the [ClockworkPi Picocalc](https://github.com/clockworkpi/PicoCalc)! 

## Why is this? 🐛
 ClockworkPi generously provides original CAD files, but these are optimized for injection molding, with draft angles and injection-molded features that complicate modification in CAD programs like SolidWorks or OpenSCAD. This also prevents perpendicular surfaces necessary for clean FFF 3D printing. 

To alleviate this I have reverse engineered the back case using my Picocalc and the .step model from Clockworkpi as a guide. After over 200 grams of test prints, the new case back is tuned as a drop-in replacement.  The SD card, 3.5 TRS jack, volume wheel, etc. all fit with no filing or fighting, the bolt pattern aligning naturally. The standard steel DIN912 M3x8 screws provided with the Picocalc is also perfectly compatible with this case back. 

## Improvements 📈
![frontal_green_labeled.jpg](/resources/images/frontal_green_labeled.jpg)
All versions of the model incorporate a new support bridge near the center in the area between the keyboard and screen.  This was done to add new hardware mounting points but also improves keyboard feel by giving it support at its top edge vastly improving key to key feel consistency. 

## Variants 🎨
![3_4_rear_labeled_green.jpg](/resources/images/3_4_rear_labeled_green.jpg)
There are a few variants of the model that I have provided in this repository.  They are to serve as a basis for anyone else who would like to build a custom back cover or serve as a drop in replacement if user requirements are met.

##### Model A:
This model is only the first ~5 mm of the case and is meant to serve as a basis for any custom designs.  The back surface is completely flat making it easier to modify than cutting and adding to the OEM .step model. 


##### Model B:
Optimized for the Picocalc with a Luckfox Lyra.  The case is 3mm deeper and incorporates two antenna ports on the top surface (SMA).  It is a two piece model which requires hardware.  Splitting the back cover and back frame allows for optimized clean printing and easy access at the cost of more hardware. Parts needed are listed in BOM under resources/BOM_Picocalc_case_back_1b.csv. 

A landing feature was also incoorporated by the 0.1" header pins for easy mounting of PCB addon cards with an M2 threaded insert for support.

Back cover consists of a printed in-place live hinge rated for approximately 50–100 open/close cycles before material fatigue becomes an issue. Held down with M3 thumbscrews for easy access.

##### Model C:
Similar to Model B but with added corner bumpers to improve durability of device against hits.  Also replaces left antenna port with a TA4F style connector cutout for non-compliant but ruggedized USB output when using the Luckfox Lyra.  Model is meant to show extensibility and possibilities with this case back family.

## Remarks ⚠️
All parts are offered in either a .step file for easy ingestion into CAD programs and workflows. They are also offered in a .stl file made for direct import into a slicer.

Two models of back plate are also offered, one with a sundial vent reminscent of Clockwork's name. The other is blank for easy customization. 

Dimensions for daughter card are provided in resources\Daughter_card_dimensions.pdf.

##### Notes on 3D Printing:
All prints and tests were done in PETG on a well trammed Ender 3V2 with slower speeds (30-50 mm/s). .2mm slicing height. PEI textured plate with a 5mm brim.  Ideally printed with widest surface facing the buildplate like a pyramid. This hides all supported surfaces inside the case. 

A key post processing step is sanding the power button lightly on the front case facing surface.  If skipped the power button will bind against the case sandwich when torqued down.  By using a draw filing technique with a narrow strip of emory paper (320 grit) adhered to a tongue depressor, a consistent surface finish can be achieved while removing all interference.  This step is best done before breaking the live hinge free.


##### Example Photos 📷
![4in1_example.jpg](/resources/images/4in1_example.jpg)



##  Next Steps👷
- Document and writeup DS3231 RTC integration with Luckfox Lyra only using Python utilizing a lightweight driver by [owainm713](https://github.com/owainm713/DS3231RTC-Python-Module).  <br>
- Integrating a National Instruments GPIB-USB-HS. <br>
- A scroll wheel? 🛞

## Thanks to, 🙌
ClockworkPi forum users:<br>
hispoot: for getting the Lyra working on the Picocalc.<br>
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
