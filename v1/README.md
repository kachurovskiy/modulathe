# modulathe v1

![modulathe v1](https://github.com/user-attachments/assets/4bb456a1-8b5c-49c3-94b5-cf9471b4e1f0)

Decide the bed length of your future lathe. By default it's 680mm. It affects:

- length of the base pipe (680mm default)
- length of the long pair of 15mm rails (500mm default)
- length of the long leadscrew (500mm default)

You can increase or decrease all of the above lengths together in steps of 50mm.

Any printed parts can be modified using FreeCAD 1.0, models in the [freecad](freecad) folder. Prints done with PETG 100% infill.

M5 (10mm 100 pcs.) and M4 (8mm 50 pcs.) threaded inserts would be used, available for 10€ on AliExpress.

M5 and M4 cylinder head bolts of various lengths are needed, get pack of 50 of each length - 12mm, 16mm, 20mm, 25mm, 30mm, 35mm.

## Preparing the steel tube

- [160x80x4mm steel tube](https://www.ebay.de/itm/132751662693?var=432062251186), 28€
- Optional [4 rubber feet 38xM8x15mm](https://www.aliexpress.com/item/1005006179757754.html), 8€

1. Cut to length (default 680mm)
2. Cleaned with an angle grinder outside removing the mill scale
3. Degreasing inside to improve concrete adhesion
4. Checked with a construction level covered with a thin film of paint for flatness, any bulges on the top surface hammered in or ground off

Rubber feet connect to the tube through [2 printed cross-members](step/Pipe160CrossFoot38M8.step) that will later be epoxied to the tube at the same time as the bed.

Tube ends are closed using the printed [end caps](step/Pipe160x80Cap1.step) which hold on friction. These caps are also used later during the concrete fill.

NOTE: you can use [heavy alu profile 160x80mm](https://www.myaluprofil.de/Aluminiumprofil-160x80-Schwer-Nut-8--I-Typ-kompatibel.html?language=en) instead, it's more expensive but needs no cutting, cleaning or grinding.

## Bed printing

- [11kg PETG filament](https://www.ebay.de/itm/354057573174?var=624933263557), 109€

If everything prints on the first try you might only need 6kg of filament for all prints.

Split the bed in 3 pieces avoiding cuts on bolt holes [using e.g. Bambu cut tool](https://wiki.bambulab.com/en/software/bambu-studio/cut-tool). **Print vertically.** Side facing the bed will get the worst geomety, orient accordingly.

- Enable 15mm adhesion brim
- Check how much your filament shrinks once printed, scaling 100.15% helped in my case

Print post-processing:

- Use woodworking chisel to shave off brim and imperfections
- Glue 200-300 grit sandpaper to a flat surface e.g. plywood or laminate, sand all 6 sides of all prints lightly with a few drops of water

https://github.com/user-attachments/assets/2fffe1df-2432-4740-9166-945ec31d264c

## Bed preparation

Melt in threaded inserts from the bottom and the sides - not from the top. Ensure they are flush or below the surface. M4 inserts on the bottom are optional, they are intended to accept grub screws that can be used to level the bed while glueing it to the steel tube.

Glue bed from the pieces together 1 connection at the time aiming for the top side surface flatness. Bottom surface of the resulting part can be uneven, it doesn't matter.

Use a clean flat surface and layers of packaging tape (mine is 0.04mm thick) to perfectly align the 2 parts.

Wait until epoxy is no longer flowing (approx 1hr) before applying it so that it doesn't leak out. Once cured, cut off the excess epoxy with a chisel.

https://github.com/user-attachments/assets/5a579cde-1618-4fe0-a3cb-860afe8003b4

## Headstock

- [High-strength small grain self-compacting concrete](https://grey-element.shop/Hochfester-Vergussbeton-10Kg), 23€
- [Vibration motor](https://www.aliexpress.com/item/1005007594000699.html), 27€
- [30mm forstner bit](https://www.aliexpress.com/item/1005007128346762.html), 11€

![image](https://github.com/user-attachments/assets/52cc1e21-6280-4ab6-b42d-b039f7f4a52d)

See https://www.youtube.com/shorts/znT_esMe_-g for illustration.

[Print headstock](step/HeadstockConcreteSunk125.step) on the side with 20 M5 holes with 5 wall loops, 2% gyroid infill and support for the rear bearing seat. Melt in all the inserts. Wrap the entire print in transparent packaging tape to make cleanup easy.

Make a 45mm hole on the rear side of the headstock where the motor would be with a hole saw.

Prepare a vibration plate by screwing the vibration motor to a large enough piece of plywood with foam mats on one side (vibration isolation) and a heavy metal plate on another side (added weight so that it doesn't jump around). Connecting motor via a foot pedal is very convenient since the hands will be busy.

Wear eye protection and single-use latex gloves. Cut off 5L bottle nozzle as a pouring chute, keep the other half with water and sponge for cleanup, use the cap to plug the nozzle when you finish pouring.

Prepare 7kg of concrete mix strictly according to instructions on the bag. Pour 1-2 litres at a time, vibrate for ~40s each time. Use flashlight to see the air pockets inside the print. Once air pockets stop shrinking, use a 2mm drill to create weep holes for air to come out, vibrate some more.

This kind of concrete cures quickly but allow the headstock to rest for at least a few days (week is better) before loading it.

Use a 30mm forstener bit to drill out the plastic where the threaded rod washer will be placed so that the headstock doesn't lose tension over time.

## Spindle lock

- [Polished hardened 9mm steel rod, 300mm](https://www.ebay.de/itm/333791840783?var=542864083101), 10€
- [Reamer 9mm](https://www.aliexpress.com/item/4000614485972.html), 4€

Cleanup the headstock 9mm through hole that's intended for the spindle lock pin with a 9mm reamer so that the polished rod slides through without getting stuck.

## Concrete and threaded rods

- Pre-mixed concrete 25kg, 8€
- 2 M10 threaded rods 1m, 9€

Cut 4 threaded rods pieces each 323-340mm long. **Check that the length is right for your headstock and pipe combination and there will be enough thread for nut and washer.**

Mark 4 holes for threaded rods by placing the bed in it's intended position on the pipe. Drill 4 holes under the headstock. Use 10, 11 or 12mm drill. Print [2 pipe covers](step/Pipe160x80Cap1.step) and cap 1 end of the pipe.

Prepare concrete for the volume of the pipe. Make sure to wear personal protection, cement should not be breathed in and it damages the skin within minutes. Use exact amount of water per instructions on your bag, normally the mix should be dry leaving almost no marks if it falls on the floor. Excess water will weaken the concrete.

Fix the pipe vertically so that the headstock is near top. Fill and compact the concrete in layers up to the lower threaded rod holes. Insert and align the threaded rods, fill and compact the concrete leaving 10mm empty on the top. Close with the top lid. Let it cure for several days.

## Spindle install

- [Spindle MT5 125mm 38mm hole Type B](https://www.aliexpress.com/item/1005004521050803.html), 108€
- [6210-2RS bearings](https://motionparts.de/products/6210-2rs1-skf), 14€
- [6209-2RS bearings](https://motionparts.de/products/6209-2rs1-skf), 11€
- [M45x1.5mm precision nut](https://www.aliexpress.com/item/1005004257672565.html), 15€

Cool the spindle, heat up the large bearing and slide it onto the spindle.

Protect the front bearing with [4 printed supports](step/BearingSupport61-89-10mm.step) held in place with tape. Small bearing can be pushed in place using an M10 threaded rod with 2 nuts. From the face of the spindle, put the rod through a large enough object. From the back side, apply pressure to both races of the bearing using [the printed bearing pusher](step/BearingPusher45.step). Push the bearing in place by holding M10 nut on one side and tightening another M10 nut on the other side. Do not over-tighten.

Print and install [spindle pulley](step/SpindleGear60GT3.step) with a 4x4x20mm steel key, tighten with light pressure using a M45 precision nut. Do not buy cheaper non-precision nuts.

## Chuck

- [Sanou 125mm 3-jaw chuck](https://www.aliexpress.com/item/1005005972611963.html), 62€

Very important to buy a quality SANOU chuck with ground jaws. Don't get VEVOR chucks.

## Encoder

- [600 pulse 5V optical rotary encoder](https://www.aliexpress.com/item/4001142743940.html), 18€
- [Belt GT3 267-3MGT-6](https://www.z24.de/a/40021-zahnriemen-3m-gt-gt3?breite=6&laenge=267&quantity=1), 12€

Print [encoder mount](step/EncoderMount.step) and [encoder gear](step/EncoderGear30GT3.step), install and lightly tighten the belt. You would need 3 pcs. M3 flat head bolts to connect encoder with the mount.

## Motor

- [1100W brushless sero motor](https://www.aliexpress.com/item/1005005662497179.html), 140€
- [Belt GT3 384-3MGT-9](https://www.z24.de/a/40021-zahnriemen-3m-gt-gt3?breite=9&laenge=384&quantity=1), 15€

Looks like the shape of motor controller board has changed since I bought, check if the new box fits [FreeCAD model](freecad/Motor1100Bracket.FCStd). [Pulley](step/MotorPulley30GT3.step) is 3D printed.

**Warning: this motor can start spinning on power-on depending on the knob position. It's incompatible with machining safety requirements.**

## Axis motors

- [STEPPERONLINE 3Nm NEMA23 closed loop](https://www.ebay.de/itm/314811928812), 2 pcs., 166€

There are cheaper motor options but these are reliable and quiet motors I prefer to use. Print [Z axis motor bracket](step/ZMotorMount.step), [X axis motor bracket](step/HM10-57-3DP.step), each take 4 M4 threaded inserts melted in from the back.

## Ball screws

- [SFU1204 C5 ball screw](https://www.aliexpress.com/item/1005001335646337.html) of 300mm and 500mm length, 55€
- [30mm tall nut housing, 24mm hole](https://www.aliexpress.com/item/1005006822739785.html) 2 pcs., 7€

It's critically important to get C5 quality, branded ball screws and nuts. C7 or unrated ball screws will much decrease the lathe characteristics due to 2-3x larger play and deflection.

One of the nut housings needs holes for M5 bolts drilled and counterbored, [see the model](freecad/BallNutMount2M5-3DP.FCStd). Alternatively you can just 3D print it.

## Ball screw mounts

- 4 pcs. [F10-18M axial bearings](https://www.aliexpress.com/item/1005007163457959.html)
- 2 pcs. 608-2RS bearings for tail ball screw mounts

Print Z axis [ball screw main mount](step/BK10Axial.step) and [tail mount](step/BF10.step). Main mount and X axis motor bracket each take 2 axial bearings. It's okay if it's hard to turn the ball screws initially, after a few days the high points on plastic yield a bit and they start to turn easier.

## Linear rails

- 500mm HGR15CA, 50€
- 300mm HGR15CC, 45€

Keep in mind that linear rails are not straight - best case they have a bow, worst case it's a spiral.

When installing Z rails, first align 1 rail to be horizontally flat using a straight edge, shims/light and kitchen foil which is 0.01mm thick. Then align it to be straight. **Aligning the first Z rail right is critical, entire lathe is aligned off of it.**

Off the first rail, align the second one using the indicator riding on the first rail in the same sequence.

Aligning the X axis rails is easy, just push them to the guiding edges while tightening the bolts.

## Middle plate

Print [the middle plate](step/MiddlePlate3DP.step) with supports, melt in the inserts from the bottom side, sand all sides on the plate for flatness, glue in 10x2mm magnets on 4 sides.

## CNC parts: top plate, headstock cover, toolpost

Order all parts at the same time on https://cnc.jlcpcb.com/cnc-machining-quote to save on shipping. You can chose powder-coating in any color but it adds to the price. Only top plate needs threads.

- [Top plate STEP file](step/TopPlate-NoThreads.step), [threads PDF](step/TopPlate.pdf)
- [Toolpost STEP file](step/Toolpost60-60CNC.step)

Order in default precision, it's good.

## Headstock alignment

- [16mm hardened steel precision bar 500mm](https://www.aliexpress.com/item/1005004969480490.html), 18€

I've ordered several bars and the one linked above is the best, others too bent or terrible scissor-cut.

For left-right alignment, ride an indicator on the side of the bar and find average values at the start and end. Adjust the headstock until averages are close to equal.

For up-down alignment, do the same procedure on the top of the bad. Sand down the bottom of the headstock to tilt in either direction. **This might affect your centerline and require sanding the middle plate by the same amount.**

It's critical to epoxy the headstock in place in good horizontal alignment. Vertical alignment can be micro-adjusted with 4 M10 nuts, just don't overtighten them. According to ChatGPT calculation the limit for each nut is 30Nm. Headstock plate needs to be epoxied too for better pressure distribution.

## Tailstock

- [MT2 100mm tailstock](https://www.aliexpress.com/item/1005005664958541.html), option B, 90€
- [Set of 4, HGH15CA linear rail carriage](https://www.aliexpress.com/item/4001272098866.html), 30€
- [Set of 10, M5 18mm countersunk hex bolts](https://www.aliexpress.com/item/1005002365855820.html), 4€
- [2pcs 30 T-track 40cm, 2pcs M8 Rod Handle](https://www.aliexpress.com/item/1005006225385865.html), 17€
- 16 of M4 35mm hex cylined head bolts
- 4 M8 40mm bolts
- 4 M8 threaded inserts

Print the [tailstock plate](step/TailstockPlate-NoThreads.step), sand it lightly for flatness, optionally use [tailstock holder](step/TailstockHolder.step) for storage of the tailstock off the lathe.

Bolt down the T-slots using countersunk bolts, bolt down the plate using M4 bolts, optionally through M4 washers.

Align the tailstock with the headstock using the [aligner pin](step/CenterlineFinder.step) held in the chuck or ride an indicator in the spindle over the dead center.

Ride an indicator on the ground extending shaft of the tailstock to ensure it's parallel to the rails.

## Further improvements

### CNC lathe bed and headstock

This project was originally designed to be CNCed from aluminum, you can find most components close to being ready for cutting in `freecad/AssemblyCNC.FCStd` - though it was not attempted yet so there are definitelly some mistakes in there.

### Angular ball bearings

Ball bearings currently used aren't supposed to take big axial loads and generally have a tiny bit of play in them intended to compensate for thermal expansion. With M10 nuts squishing them into ovals, it remains to be seen how long they will last.

For the next modulathe iteration I'm looking to use 3209B-2RS and 3210B-2RS angular double-row ball bearings which are heavier duty but larger.

### Wider headstock

Weakest point of all desktop lathes is sideways deflection of the chuck - not upwards deflection as it may seem. Pull on the long bar inserted into the chuck and you'll notice that it deflects front/back by 0.5mm while only deflecting 0.05mm up and down. It also depends on the chuck position so deflection oscillates on each chuck rotation creating vibrations and poor finish.

Making headstock wider, full width of the base would reduce the severity of headstock twisting, allow for larger bearings to be used and for M12 rods which can be placed on the sides of each bearing (not slightly in the back like today).

### Heavy alu profile

[Heavy alu profile 160x80mm](https://www.myaluprofil.de/Aluminiumprofil-160x80-Schwer-Nut-8--I-Typ-kompatibel.html?language=en) might be a better choise for the base. It calls for the entire design to be re-done though since it offers plenty of better fastening options.
