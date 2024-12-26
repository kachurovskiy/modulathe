# modulathe v1

![PXL_20241208_165959620-Photoroom](https://github.com/user-attachments/assets/90273628-7344-4fc4-a882-eb2a0de424a4)

Decide the bed length of your future lathe. By default it's 680mm. It affects:

- length of the base pipe (680mm default)
- length of the long pair of 15mm rails (500mm default)
- length of the long leadscrew (500mm default)

You can increase or decrease all of the above lengths together in steps of 50mm.

Any printed parts can be modified using FreeCAD 1.0, models in the [freecad](freecad) folder. Prints done with PETG 100% infill.

## Preparing the steel tube

- [160x80x4mm steel tube](https://www.ebay.de/itm/132751662693?var=432062251186), 28€
- Optional [4 rubber feet 38xM8x15mm](https://www.aliexpress.com/item/1005006179757754.html), 8€

Tube needs to be:

1. Cut to length (default 680mm)
2. Cleaned with an angle grinder outside removing the mill scale
3. Degreasing inside to improve concrete adhesion
4. Checked with a construction level for reasonable flatness, any bulges on the top surface hammered in or ground off

Rubber feet connect to the tube through [2 printed cross-members](step/Pipe160CrossFoot38M8.step) that will later be epoxied to the tube at the same time as the bed.

Tube ends are closed using the printed [end caps](step/Pipe160x80Cap1.step) which hold on friction with the inner tube weld. These caps are also used later during the concrete fill.

## Printing the bed and headstock

- [11kg PETG filament](https://www.ebay.de/itm/354057573174?var=624933263557), 109€
- M5 threaded inserts: 27 for the headstock, 11 for each HGR20 rail (2 needed during assembly), 16 for the bed (65 in total), 6€
- M4 threaded inserts: 9 for each HGR15 rail (18 total), 3€

Split [BaseAndHeadstock3DP.step](step/BaseAndHeadstock3DP.step) vertically between the bed and the headstock at 30.01mm [using e.g. Bambu cut tool](https://wiki.bambulab.com/en/software/bambu-studio/cut-tool). Split the remaining headstock vertically in the middle, then each part again with the dovetails. Split the bed in 7-8 pieces (in half, then each piece again in half) with the dovetail. Try not to split along any holes. Print with full infill.

![image](https://github.com/user-attachments/assets/db2ea30d-8c68-46e1-b515-57161092a6ba)

Most printers build volume theoretically allows to split in only 4 parts but that is not recommended:

- Headstock should not be printed in 1 part with the bed since we need to micro-adjust the headstock after the bed is glued
- Large parts shrink, pull the magnetic bed up and starts wobbling
- Bed should is split into more pieces to not exceed the magnetic base force limit
- Smaller parts mean that a potential failure is cheaper (e.g. tangled filament), less material is thrown away

Enable adhesion brim and supports for the bed side rails. Without adhesion brim, the parts will warp more.

Add support blocker to avoid unnecessary supports. Without supports for the upper lip it will print as noodles.

![image](https://github.com/user-attachments/assets/3a48ef8b-05d3-4a32-9e71-af972e6fed56)

Print post-processing:

- Use woodworking chisel to shave off any imperfections
- Use large flat file to remove bulges on the edges, sand down the layer lines a bit

It's possible to print the bed vertically in 3 pieces and it has advantages - not needing support, less warping - but the resulting parts shrink measurably and can result in the rail holes to no longer aligning.

## Headstock glue-up

- [Polished hardened 9mm steel rod, 300mm](https://www.ebay.de/itm/333791840783?var=542864083101), 10€
- [Reamer 9mm](https://www.aliexpress.com/item/4000614485972.html), 4€

Cleanup the headstock 9mm through hole that's intended for the spindle lock pin with a 9mm reamer so that the polished rod slides through without getting stuck.

Roughen, degrease the headstock mating surfaces, wet with epoxy, align with the rod and try to get the most square part possible. Once epoxy hardens, excess can be cleaned up with a chisel.

[Z motor plate](step/BaseAndHeadstock3DP-MotorPlate.step) needs M4 inserts melted in from the flat side and glued into the headstock.

## Filling headstock with sand

Wash 1 liter of sand in a bucket by filling with water, agitating and then draining the water off the side. Repeat until the water is clean, approx. 5 times.

Dry the sand thoroughly naturally and/or in the cooking pan.

Ensure the glue seam inside the rectangular headstock cavity has no holes.

Fill the rectangular headstock cavity with the sand leaving space for the lid, compact by landing the headstock on the table lightly several times.

[Print the lid](step/BaseAndHeadstock3DP-SandHoleCover.step), hammer it in flush through a large flat block so that it doesn't go in too deep.

## Bed glue-up

- Optional 2 HGR20 600mm (only needed during the glue-up or if you have plans for them), 52€

Ensure all M5 through holes in the bed have the long enough threaded inserts melted in from the bottom side.

M4 through holes for the main rails can also have inserts melted in from below.

Cover the threaded inserts on the bottom side with small patches of tape so that epoxy wouldn't get into the threads.

Install 2 side HGR20 rails and 2 HGR15 top rails for bed alignment. The geometry of the bed must not be determined by the steel tube - instead we aim to make the bed as flat as possible and lock it in place using epoxy to fill in the cavities and tube to provide stiffness.

Plastic and metal mating surfaces to be roughened with an orbital sander and degreased. Mating surfaces wetted with epoxy, bed lowered onto the tube and positioned. Do not clamp the bed to the tube. Aim for a thin epoxy layer to minimize shrinkage.

Glue will drip off the sides of the tube, protect your working surface.

HGR20 rails to be removed after the epoxy sets.

## Concrete and threaded rods

- Pre-mixed concrete 25kg, 8€
- 2 M10 threaded rods 1m, 9€

Cut 4 threaded rods pieces each 340mm long.

Drill 4 holes for threaded rods under the headstock. Use 10, 11 or 12mm drill. Print [2 pipe covers](step/Pipe160x80Cap1.step) and cap 1 end of the pipe.

Prepare concrete for the volume of the pipe. Make sure to wear personal protection, cement should not be breathed in and it damages the skin quickly. Use exact amount of water per instructions on your bag, normally the mix should be dry leaving almost no marks if it falls on the floor. Excess water will harm the results.

Fix the pipe vertically so that the headstock is near top. Cover all areas except the top hole. Fill and compact the concrete up to the lower threaded rod holes. Insert and align the threaded rods, fill and compact the concrete leaving 10mm empty on the top. Close with the top lid. Let it cure for several days.

## Spindle install

- [Spindle MT5 125mm 38mm hole Type B](https://www.aliexpress.com/item/1005004521050803.html), 108€
- [6210-2RS bearings](https://www.amazon.de/dp/B071YY8Q8C), 26€
- [6209-2RS bearings](https://www.amazon.de/dp/B071YY92JB), 25€

Cool the spindle, heat up the large bearing and slide it onto the spindle.

Cool the spindle with the large bearing and insert it into the headstock.

Small bearing can be pushed in place using an M10 threaded rod with 2 nuts. From the face of the spindle, put the rod through a large enough object. From the back side, apply pressure to both races of the bearing using [the printed bearing pusher](step/BearingPusher45.step). Push the bearing in place by holding M10 nut on one side and tightening another M10 nut on the other side. Do not over-tighten as excessive axial load can damage the front bearing.

## Additional anti-vibration measure

- Optional [2 pads of 12.7cm Sorbothane 70 Duro](https://www.amazon.de/dp/B005JRO1KO?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1), 83€

Sorbothane pads are alternative to the rubber feet and supposedly remove 95% of vibrations. I didn't test their effectiveness yet. Hard to peel them off, might not be reusable, less clearance for picking up the lathe compared to feet.
