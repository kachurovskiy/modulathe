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

- 910 EUR in large items detailed below
- 290 EUR for CNC middle plate, top plate, tool holder cube
- 110 EUR for the aluminum CNC tailstock plate (optional)

Not counting motors, controller, concrete or rebar.

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

### Other 194 EUR

- [10kg of PETG](https://www.ebay.de/itm/354057573174?var=624933263556) - 108 EUR
- [2 packs of M5 inserts 10mm length, outside diameter 7mm, 100Pcs](https://www.aliexpress.com/item/1005006798286851.html) - 15 EUR
- [M8 inserts 12mm length, outside diameter 10mm, 10Pcs](https://www.aliexpress.com/item/1005008666672949.html) - 2 EUR
- [Large 120 grit diamond plate](https://www.aliexpress.com/item/1005007177296408.html) - 10 EUR
- [Wet sandpaper 5pcs, 230x280mm, 240 grit](https://www.aliexpress.com/item/1005005510517824.html) - 6 EUR
- [4x rubber feet 38xM8x15mm](https://www.aliexpress.com/item/1005006179757754.html) - 7 EUR
- [Straight edge 300mm](https://www.aliexpress.com/item/4000846597491.html) - 34 EUR
- [Feeler gauge](https://www.aliexpress.com/item/1005007758368050.html) - 3 EUR
- [Bees wax](https://www.amazon.de/-/en/dp/B09QPRQ531) - 9 EUR

## Using epoxy

Standard 2-component epoxy is used to glue the bed molds together, seal concrete parts and glue aligned head to the bed.

Always lightly sand and clean the parts with isopropanol before epoxying. Remove excess wet expoxy with paper towels, excess dry epoxy with a woodworking chisel. If the glued gaps are large, wait 30m for epoxy to increase viscosity before use.

Always wear gloves, glasses and other protective equipment when working with epoxy, it's very allergic.

## 3D printing preparation

### Calibration

Ensure that your printer produces accurate parts e.g. print a 100mm cube and cylinder with standard infill and check how far the dimensions are from 100mm.
Don't forget to check the height, too. Adjust the slicer settings so that your future prints come out precise. Even a 0.5% error might result in linear rail holes being unusable for a long rail.

### Plastic to use

[10kg set of PETG rolls](https://www.ebay.de/itm/354057573174?var=624933263556) - printing all molds takes much less than that but it gives you a chance to re-print in case of mistakes.

### Print settings

Always print with adhesion layer to reduce the risk of mold deformation during printing. Most molds are printed vertically with standard settings. Molds going inside the spindle are printed with 100% infill to be able to pull the bearings out.

### Chamber temperature

For good part geometry it's critical to maintain high, constant printing chamber temperature throughout the printing process and let the print cool slowly. Additional outside insulation of the printing chamber is necessary. It's much better to print a good mold than to fix a concrete part.

### Sanding plate for the molds

Get a large, quality 240 grit sandpaper e.g. https://www.aliexpress.com/item/1005005510517824.html and glue it on a flat piece of water-resistant MDF or plywood with double-sided tape. Avoid tape gaps behind the sandpaper. All flat sides of 3D prints are to be lightly sanded with a spray of water for a better fit.

### Adaptive layer height

Take advantage of slicers ability to reduce layer height when printing overhangs for better quality without the use of supports.

## Molds

### Bed

Print [Bed-MoldTop800.step](step/Bed-MoldTop800.step) vertically split into 3 parts. No supports should be needed.

Print 8 [Bed-MoldConnector.step](step/Bed-MoldConnector.step) to align the bed pieces together while gluing them with epoxy.

Print 4 [Bed-Spoke.step](step/Bed-Spoke.step) and epoxy them into the main bed mold. Make sure they stand straight and flush.

Print 38x [Head-DepthSpacer5.step](step/Head-DepthSpacer5.step) for later use.

Before gluing the mold, make sure that the rail holes in the mold match ones on your HGR20 rails. If mold holes are too close together, print thin shims to compensate.

When gluing the mold together, it's not necessary to squeese it tight, connectors should hold it. Instead focus on gluing it straight to reduce post-processing.

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

### Tailstock

Print [TailstockPlate-Mold.step](step/TailstockPlate-Mold.step) horizontally. Check that your vertical cylinders representing future bolt holes aren't undersized to be used for M5 and M8 bolts.

Melt in 4 M5 threaded inserts from the inside, cover them with pieces of sticky tape so that concrete wouldn't get in.

### Waxing

Ensure all glued parts of the molds are in place before waxing.

Treat all mold surfaces that will be touching concrete with bees wax.

### In-concrete threaded inserts

Inserts have to be free of wax so they're installed after waxing.

- Bed needs 38 M5 inserts
- Head needs 68 M5 inserts
- Tailstock needs 4 M8 inserts

Each insert is installed in place with a 25mm M5 cylinder bolt - 10mm goes to wall thickness, 5mm to plastic standoff and 10mm to threaded insert.

For every M5 insert, don't forget to first install the `Head-DepthSpacer5.step` standoffs you printed previously. Without them, threaded insert will have minimal holding power.

If your bolt is too short, concrete will get into the threaded insert and make its usable depth smaller. If the bolt is too long, you might not be able to unscrew it once the concrete sets.

Normally there's no need to wax the ends of the bolts, concrete won't stick to them.

## Concrete

### Volume calculation

- Bed is 8.9 litres
- Headstock is 4.62 litres
- Tailstock plate is 1.23 litres

If you're pouring all 3 parts, total is approx. 15 litres of concrete.

If you modify any of the parts, it's easy to measure volume of updated parts by opening the corresponding STEP file in 3D slicer that shows volume in cubic millimeters.

### Mix design

Mix requirements:

- High compressive strength - at least 50 MPa
- High tensile strength - at least 10 MPa
- Has sufficient maximal layer thickness of at least 160mm
- Does not require exotic equipment to mix and pour

This rules out most or all of the home improvements bagged concrete since those mixes are usually around 10 MPa in compression and unrated for tensile stress.

Having tried and being disappointed by some of the consumer-graded mixes on Amazon, I recommend going with professional mixes only. Do a small test pour and check compressive and tensile strength when in doubt.

Standard concrete mixes shrink when cured - outside dimensions get smaller, inside holes get larger. Headstock bearings are easy to remove from shrinking mixes but they also don't hold much on friction and require some countermeasures.

There are special expanding concrete mixes that slightly increase in side as they cure. Headstock bearings are hard to remove but they also hold very well just on friction.

[SikaGrout-234 high-performance vibration-resistant expanding grout](https://tun.sika.com/dms/getdocument.get/a8b219c4-161c-44d6-b310-b7932fb5eb68/sikagrout-234.pdf) is what I used in my build. It produces 12.5L of product and can be supplemented with 2.5L of e.g. washed basalt gravel under 8mm. Use precisely the specified amount of water.

### Reinforcement

I didn't use any reinforcement - basalt fibers make the mix hard to compact and I forgot about steel rebar.

Ideally there would be reinforcement embedded into the mix and additonally a space for two M12 rods to insert into the base after curing for post-tensioning.

### Compaction

Consider using a submersible concrete vibrator, they're cheap on AliExpress - just beware of the concrete splashing all over the place when you run it. I used a table with vibration motor but it only worked on the tailstock mold, other molds were too heavy for it.

### Working surface for the molds

Concrete is very heavy and you might end up with a bent bed if the bed mold is filled on an uneven surface or if the weight of concrete can deform the table with the mold.

### Embedding bed feet into the concrete

It might seem like you can just place the rubber feet into the wet concrete with M8 threded inserts attached but they will start sinking at an angle. It would be beneficial to have each pair of feet attached to a thin flat platform when curing.

### Safety

Concrete is very dangerous in both dry and wet forms, use appropriate protection and prevention measures e.g. vacuum up the airborne dust, cover skin, use waterproof gloves and face protection.

### Curing

Wrap the molds in plastic after the pour to keep the moisture in the mix for proper curing.
