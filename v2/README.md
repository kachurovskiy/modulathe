This software and instructions are [provided as is](../LICENSE), without warranty of any kind. [Lathes are dangerous.](https://www.worksafe.vic.gov.au/safe-use-metal-turning-lathes)

# Modulathe V2

**NOTE: this version is still a work in progress, below is the provisinal documentation.**

free and open-source metal lathe design where we print the forms using a 3D printer, fill them with concrete or other suitable mix, post-process the parts with sanding and assemble a CNC-ready lathe together using off-the-shelf parts and a few custom CNCed pieces.

- 125mm chuck, MT5 spindle with 38mm through-hole
- 136mm cross-slide travel
- 80mm between cross-slide and centerline
- 300mm maximum turning diameter
- Any bed length, default 800mm with 600mm rails
- No backlash, double ball nut on Z
- 20mm/15mm linear rails, 16mm/12mm ball screws, NEMA23 motors
- Double row angular ball bearings
- Integrated spindle lock and magnet bed covers
- Manual operation and CNC with or without PC

It is a hard, long and expensive project to complete. The end result can surpass many comparable lathes in rigidity and features.

## Core ideas

- Commercial CNC lathes are too expensive, heavy, complicated, vendor-locked, hard to repair
- Commercial manual lathes use antiquated tech with most parts needing replacement for a CNC upgrade
- Mass-produced precision parts (motors, linear rails, ball screws) are cheap
- Precision lathe body can be achieved with 3D-printed molds and post-processing
- Rigidity can be achieved by using concrete, high performance grouts or epoxy granite
- Custom metal parts can be ordered online for reasonable money
- [DIY digital lathe controllers exist](https://github.com/kachurovskiy/nanoels)
- Select and modify the modules - motors, bed length, tool posts, bearings
- Iterate and improve, share your knowledge and results for others to reproduce

## Audience

- People who like to make their own tools
- 3D printing enthusiasts looking to expand their machine park
- Craftsmen with specific requirements unmet by the commercially available lathes

People who's needs might not be met by this project:

- Need a good lathe quickly to get actual work done
- Need to feel the pressure feedback on the handwheels
- Need a machine meeting local machinery regulations

## Finding files and models

STEP files that can be directrly used in 3D printer slicers and to order CNC parts: https://github.com/kachurovskiy/modulathe/tree/master/v2/step - several PDF files in there too for CNC parts with threads

FreeCAD models that can be used to modify certain parts: https://github.com/kachurovskiy/modulathe/tree/master/v2/freecad - see Assembly.FCStd for the overall picture.

## Bill of materials

About 910 EUR in large items, not including concrete, motors or controller.

400 EUR more for CNC parts (middle plate, top plate, tailstock plate, tool holder cube).

### Spindle 242 EUR

- [Sanou 125mm self-centering chuck](https://www.aliexpress.com/item/1005007987289683.html) - 42 EUR
- [MT5 spindle with 38mm hole, Type B](https://www.aliexpress.com/item/1005004521050803.html) - 98 EUR
- [Spindle nut, Pitch 1.5mm, R M45](https://www.aliexpress.com/item/1005004257672565.html) - 12 EUR
- [3209 B 2RSRTNG NSK](https://motionparts.de/en/products/3209-b-2rsrtng-nsk) - 41 EUR
- [3210 B 2RSRTNG NSK](https://motionparts.de/en/products/3210-b-2rsrtng-nsk) - 49 EUR

### Z axis 192 EUR

- [DFU1605 C5 ballscrew, 600mm](https://www.aliexpress.com/item/1005004126133993.html) - 85 EUR
- [HGR20 600mm with 4x HGH20CA](https://www.aliexpress.com/item/1005006571096820.html) - 80 EUR
- [HM12-57 C5 motor mount](https://www.aliexpress.com/item/1005007378312793.html) - 27 EUR

### X axis 122 EUR

- [SFU1204 C5 ballscrew, 300mm](https://www.aliexpress.com/item/1005001335646337.html) - 22 EUR
- [HGR15 300mm with 4x HGW15CC](https://www.aliexpress.com/item/1005006571096820.html) - 57 EUR
- [HM10-57 C5 motor mount](https://www.aliexpress.com/item/1005005236581474.html) - 32 EUR
- [BF10 ball screw tail mount](https://www.aliexpress.com/item/32717973925.html) - 8 EUR
- [Nut housing 24mm](https://www.aliexpress.com/item/1005006822739785.html) - 3 EUR

### Tailstock 165 EUR

- [MT2 tailstock 100m, Type B](https://www.aliexpress.com/item/1005007709575532.html) - 98 EUR
- [4x HGH20CA](https://www.aliexpress.com/item/1005005705301031.html) - 47 EUR
- [30mm T-track 40cm](https://www.aliexpress.com/item/1005006225385865.html) - 14 EUR
- [T-track 2pcs T Screw Handle](https://www.aliexpress.com/item/1005006225385865.html) - 6 EUR

### Other 192 EUR

- [10kg of PETG](https://www.ebay.de/itm/354057573174?var=624933263556) - 108 EUR
- [2 packs of M5 inserts 10mm length, outside diameter 7mm, 100Pcs](https://www.aliexpress.com/item/1005006798286851.html) - 15 EUR
- [Large 120 grit diamond plate](https://www.aliexpress.com/item/1005007177296408.html) - 10 EUR
- [Wet sandpaper 5pcs, 230x280mm, 240 grit](https://www.aliexpress.com/item/1005005510517824.html) - 6 EUR
- [4x rubber feet 38xM8x15mm](https://www.aliexpress.com/item/1005006179757754.html) - 7 EUR
- [Straight edge 300mm](https://www.aliexpress.com/item/4000846597491.html) - 34 EUR
- [Feeler gauge](https://www.aliexpress.com/item/1005007758368050.html) - 3 EUR
- [Bees wax](https://www.amazon.de/-/en/dp/B09QPRQ531) - 9 EUR

## Using epoxy

Standard 2-component epoxy is used to glue the bed molds together, seal concrete parts and glue aligned head to the bed.

Always lightly sand and clean the parts with isopropanol before epoxying. Remove excess epoxy with a woodworking chisel. Wait 30m for epoxy to increase viscosity if the gaps are large.

Always wear gloves, glasses and other protective equipment when working with epoxy, it's very allergic.

## 3D printing preparation

### Calibration

Ensure that your printer produces accurate parts e.g. print a 100mm cube and cylinder with standard infill and check how far the dimensions are from 100mm.
Don't forget to check the height, too. Adjust the slicer settings so that your future prints come out precise. Even a 0.5% error might result in linear rail holes being unusable for a long rail.

### Plastic to use

10kg set of PETG rolls e.g. https://www.ebay.de/itm/354057573174?var=624933263556

### Print settings

Always print with adhesion layer to reduce the risk of mold deformation during printing. Most molds are printed vertically with standard settings. Molds going inside the spindle are printed with 100% infill to be able to pull the bearings out.

### Chamber temperature

For good part geometry it's critical to maintain high, constant printing chamber temperature throughout the printing process and let the print cool slowly. Additional outside insulation of the printing chamber is necessary.

### Sanding plate for the molds

Get a large, quality 240 grit sandpaper e.g. https://www.aliexpress.com/item/1005005510517824.html and glue it on a flat piece of water-resistant MDF or plywood with double-sided tape. Avoid tape gaps behind the sandpaper. All flat sides of 3D prints are to be lightly sanded with a spray of water for a better fit.

## Molds

### Bed

Print [Bed-MoldTop800.step](step/Bed-MoldTop800.step) vertically split into 3 parts. No supports should be needed.

Print 8 [Bed-MoldConnector.step](step/Bed-MoldConnector.step) to align the bed pieces together while gluing them with epoxy.

Print 4 [Bed-Spoke.step](step/Bed-Spoke.step) and epoxy them into the main bed mold. Make sure they stand straight and flush.

Before gluing the mold, make sure that the rail holes in the mold match ones on your HGR20 rails. If mold holes are too close together, print thin shims to compensate.

When gluing the mold together, it's not necessary to squeese it tight, connectors should hold it. Instead focus on glueing it straight to reduce post-processing.

### Head

Print the following parts, vertically without supports:

- [Head-MoldBack.step](step/Head-MoldBack.step)
- [Head-MoldFront.step](step/Head-MoldFront.step)
- [Head-MoldMotor.step](step/Head-MoldMotor.step)
- 2x [Head-MoldSide.step](step/Head-MoldSide.step)
- 4x [Head-MoldSpoke.step](step/Head-MoldSpoke.step)
- [Head-SpindleStop.step](step/Head-SpindleStop.step)
- 2x [Head-StopHolder.step](step/Head-StopHolder.step)
- 68x [Head-DepthSpacer5.step](step/Head-DepthSpacer5.step)

These ones are suggested to be printed horizontally:

- [Head-MoldTop.step](step/Head-MoldTop.step)
- [Head-Spider.step](step/Head-Spider.step)

Vertically with 100% infill:

- [Head-SpindleBack.step](step/Head-SpindleBack.step)
- [Head-SpindleFront.step](step/Head-SpindleFront.step)

Melt in 38 M5 threaded inserts into back, front, side and motor molds. When melting in an insert, make sure it's a tiny bit below the surface - this allows the bolt to transfer more pressure.

Sand the molds lightly to improve surface quality.

Glue 4 Head-MoldSpoke.step into the Head-MoldTop.step flush with the open end of the mold so that they don't start moving during the concrete pour.

Treat all mold surfaces that will be touching concrete with bees wax.
