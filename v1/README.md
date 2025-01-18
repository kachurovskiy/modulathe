# modulathe v1

![image](https://github.com/user-attachments/assets/865b4746-161d-4c95-9fc8-a569a91396af)

Decide the bed length of your future lathe. By default it's 680mm. It affects:

- length of the base pipe (680mm default)
- length of the long pair of 15mm rails (500mm default)
- length of the long leadscrew (500mm default)

You can increase or decrease all of the above lengths together in steps of 50mm.

Any printed parts can be modified using FreeCAD 1.0, models in the [freecad](freecad) folder. Prints done with PETG 100% infill.

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

## Printing the bed and headstock

- [11kg PETG filament](https://www.ebay.de/itm/354057573174?var=624933263557), 109€

Split [BaseAndHeadstock3DP.step](step/BaseAndHeadstock3DP.step) vertically between the bed and the headstock at 30.01mm [using e.g. Bambu cut tool](https://wiki.bambulab.com/en/software/bambu-studio/cut-tool). Split the bed in 3 pieces avoiding cuts on bolt holes. Side facing the bed will get the worst geomety, orient accordingly.

![image](https://github.com/user-attachments/assets/0efe83ff-15fc-455f-9503-fa06ed7b5852)

- Enable 15mm adhesion brim
- Enable support for the headstock rear bearing seat
- Check how much your filament shrinks once printed, scaling 100.15% helped in my case

Print post-processing:

- Use woodworking chisel to shave off brim and imperfections
- Glue 200-300 grit sandpaper to a flat surface e.g. plywood or laminate, sand all 6 sides of all prints lightly with a few drops of water

https://github.com/user-attachments/assets/2fffe1df-2432-4740-9166-945ec31d264c

## Spindle lock

- [Polished hardened 9mm steel rod, 300mm](https://www.ebay.de/itm/333791840783?var=542864083101), 10€
- [Reamer 9mm](https://www.aliexpress.com/item/4000614485972.html), 4€

Cleanup the headstock 9mm through hole that's intended for the spindle lock pin with a 9mm reamer so that the polished rod slides through without getting stuck.

## Headstock preparation

- M5 threaded inserts: 27, 6€

[Z motor plate](step/BaseAndHeadstock3DP-MotorPlate.step) needs four M4 inserts melted in from the flat side and glued into the headstock.

Wash 1 liter of sand in a bucket by filling with water, agitating and then draining the water off the side. Repeat until the water is clean, approx. 5 times.

Dry the sand thoroughly naturally and/or in the cooking pan.

Fill the rectangular headstock cavity with the sand leaving space for the lid, compact by landing the headstock on the table lightly several times.

[Print the lid](step/BaseAndHeadstock3DP-SandHoleCover.step), hammer it in flush through a large flat block so that it doesn't go in too deep.

Alternatively, mix some epoxy, wait 1hr for it to get the consistency of a sour cream and place on top of the sand forming a seal. Free sand is supposedly better at absorbing vibtations than epoxy-bound sand.

## Bed preparation

- M5 threaded inserts: approx. 50, 6€
- M4 threaded inserts: approx. 50, 4€
- M4 8mm grub screws: 24, 3€

Melt in threaded inserts from the bottom and the sides - not from the top. Ensure they are flush or below the surface.

Glue bed from the pieces together 1 connection at the time aiming for the top side surface flatness. Bottom surface of the resulting part can be uneven, it doesn't matter.

Use a clean flat surface and layers of packaging tape (mine is 0.04mm thick) to perfectly align the 2 parts.

Wait until epoxy is no longer flowing (approx 1hr) before applying it so that it doesn't leak out. Once cured, cut off the excess epoxy with a chisel.

https://github.com/user-attachments/assets/5a579cde-1618-4fe0-a3cb-860afe8003b4

## Concrete and threaded rods

- Pre-mixed concrete 25kg, 8€
- 2 M10 threaded rods 1m, 9€

Cut 4 threaded rods pieces each 340mm long.

Mark 4 holes for threaded rods by placing the bed in it's intended position on the pipe. Drill 4 holes under the headstock. Use 10, 11 or 12mm drill. Print [2 pipe covers](step/Pipe160x80Cap1.step) and cap 1 end of the pipe.

Prepare concrete for the volume of the pipe. Make sure to wear personal protection, cement should not be breathed in and it damages the skin within minutes. Use exact amount of water per instructions on your bag, normally the mix should be dry leaving almost no marks if it falls on the floor. Excess water will weaken the concrete.

Fix the pipe vertically so that the headstock is near top. Fill and compact the concrete up to the lower threaded rod holes. Insert and align the threaded rods, fill and compact the concrete leaving 10mm empty on the top. Close with the top lid. Let it cure for several days.

## Spindle install

- [Spindle MT5 125mm 38mm hole Type B](https://www.aliexpress.com/item/1005004521050803.html), 108€
- [6210-2RS bearings](https://motionparts.de/products/6210-2rs1-skf), 14€
- [6209-2RS bearings](https://motionparts.de/products/6209-2rs1-skf), 11€

Cool the spindle, heat up the large bearing and slide it onto the spindle.

Protect the front bearing with [4 printed supports](step/BearingSupport61-89-10mm.step) held in place with tape. Small bearing can be pushed in place using an M10 threaded rod with 2 nuts. From the face of the spindle, put the rod through a large enough object. From the back side, apply pressure to both races of the bearing using [the printed bearing pusher](step/BearingPusher45.step). Push the bearing in place by holding M10 nut on one side and tightening another M10 nut on the other side. Do not over-tighten.

## Further links and instructions

To be added in the coming weeks. In summary it's HGR15 rails, 1204 ball screws from AliExpress in C5 quality. Cross-slide plate ordered from JLCPCB with threads done by them according to the PDF in the `step` package. Ball screw mounting blocks 3D printed with axial bearings. All other models are already shared.

## Additional anti-vibration measure

- Optional [2 pads of 12.7cm Sorbothane 70 Duro](https://www.amazon.de/dp/B005JRO1KO?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1), 83€

Sorbothane pads are alternative to the rubber feet and supposedly remove 95% of vibrations. I didn't test their effectiveness yet. Hard to peel them off, might not be reusable, less clearance for picking up the lathe compared to feet.
