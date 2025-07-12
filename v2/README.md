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

## Printing the molds

### Bed

Print [Bed-MoldTop800.step](step/Bed-MoldTop800.step) vertically split into 3 parts. No supports should be needed.

Print 8 [Bed-MoldConnector.step](step/Bed-MoldConnector.step) to align the bed pieces together while gluing them with epoxy.

Print 4 [Bed-Spoke.step](step/Bed-Spoke.step) and epoxy them into the main bed mold. Make sure they stand straight and flush.

### Head

To be continued.
