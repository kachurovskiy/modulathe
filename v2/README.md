# Modulathe V2

NOTE: this version is still a work in progress, below is the provisinal documentation.

## Summary

Modulathe V2 is a free and open-source metal lathe design where we print the forms using a 3D printer, fill them with concrete or other suitable mix, post-process the parts with sanding and assemble a CNC-ready lathe together using off-the-shelf parts and a few custom CNCed pieces.

It is a hard, long and expensive project to complete. The end result can surpass many comparable lathes in rigidity and features. Project is also easy to customize e.g. to increase the bed length.

## Finding files and models

STEP files that can be directrly used in 3D printer slicers and to order CNC parts: https://github.com/kachurovskiy/modulathe/tree/master/v2/step - several PDF files in there too for CNC parts with threads

FreeCAD models that can be used to modify certain parts: https://github.com/kachurovskiy/modulathe/tree/master/v2/freecad - see Assembly.FCStd for the overall picture

## 3D printing preparation

### Calibration

Ensure that your printer produces accurate parts e.g. print a 100mm cube and cylinder with standard infill and check how far the dimensions are from 100mm.
Don't forget to check the height, too. Adjust the slicer settings so that your future prints come out precise. Even a 0.5% error might result in linear rail holes being unusable for a long rail.

### Plastic to use

Getting a 10kg set of PETG rolls is recommended e.g. https://www.ebay.de/itm/354057573174?var=624933263556

### Print settings

Always print with adhesion layer to reduce the risk of mold deformation during printing. Most molds are printed vertically with standard settings. Molds going inside the spindle are printed with 100% infill to be able to pull the bearings out.

### Sanding plate for the molds

Get a large, quality 240 grit sandpaper e.g. https://www.aliexpress.com/item/1005005510517824.html and glue it on a flat piece of water-resistant MDF or plywood with double-sided tape. Avoid tape gaps behind the sandpaper. All flat sides of 3D prints are to be lightly sanded with a spray of water for a better fit.

## Printing the molds

### Bed

Print [Bed-MoldTop800.step](https://github.com/kachurovskiy/modulathe/blob/master/v2/step/Bed-MoldTop800.step) vertically split into 3 parts. No supports should be needed.

You would need 8 [Bed-MoldConnector.step](https://github.com/kachurovskiy/modulathe/blob/master/v2/step/Bed-MoldConnector.step) to connect them together.

Print 4 [Bed-Spoke.step](https://github.com/kachurovskiy/modulathe/blob/master/v2/step/Bed-Spoke.step) and epoxy them into the main bed mold. Make sure they stand straight and flush.

### Head

To be continued.
