# PCB manufacturing

This is a simple guide (and a reference for me in the future) to make simple PCBs at home. Other than the actual materials used for the synthesis, a resin printer is required.

# BOM

|Item   |Store   |
|---|---|
|Single sided copper clad boards   |[link](https://www.amazon.it/gp/product/B07RBK9WW6/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1)   |
|Photosensitive film   |[link](https://www.amazon.it/gp/product/B07YG6GY8M/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&psc=1)   |
|Ferric Chloride   |[   |
|Sodium Carbonate (soda ash or washing soda)   |   |
|Acetone   |   |

# Tools

- Resin printer
- Drill press (strongly recommended but you can even do it by hand with bad results)
- Scoring board
- Ruler
- Cutter

# Prepare the PCB

For this guide I will refer to [easyEDA] (https://easyeda.com/).

Once you have the PCB that you want to synthesize:

## [Workflow with Easyeda](https://app.tango.us/app/workflow/90083be7-d5cb-4119-86ca-6c27e43ff477?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)


__Source:__ [Tango](https://app.tango.us/app/workflow/90083be7-d5cb-4119-86ca-6c27e43ff477?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)

***

### 1. File > Export > SVG...
![Step 1 screenshot](https://images.tango.us/public/screenshot_5b48715f-c5c7-4f96-8201-55a2fd0322ed.png?crop=focalpoint&fit=crop&fp-x=0.1963&fp-y=0.1961&fp-z=2.5464&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A877)


### 2. Drag the dropdown menu and select "2.5x", leave the other settings as shown in the image
![Step 2 screenshot](https://images.tango.us/public/screenshot_540111e0-dd72-431f-a839-5487249c6629.png?crop=focalpoint&fit=crop&fp-x=0.5305&fp-y=0.2822&fp-z=2.7907&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A877)


### 3. Uncheck "Bottom layer screen printing"
![Step 3 screenshot](https://images.tango.us/public/screenshot_ba9b7e0a-489e-4bbd-9679-9228618983df.png?crop=focalpoint&fit=crop&fp-x=0.5049&fp-y=0.5398&fp-z=3.1780&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A877)


### 4. Click on "Export"
![Step 4 screenshot](https://images.tango.us/public/screenshot_53427cc1-2d64-4bd9-9693-c4e5c0c0f933.png?crop=focalpoint&fit=crop&fp-x=0.5487&fp-y=0.8478&fp-z=2.9313&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A877)


***
_[This Workflow was created with Tango](https://app.tango.us/app/workflow/90083be7-d5cb-4119-86ca-6c27e43ff477?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)_
# Prepare the board

The first thing to do is clean the card. I usually rub the copper clad board with fine grain sanding paper (320-400 grit) to even the surface and remove the stains; do not overdo it because the copper film is thin and could wear out too much, making the traces too thin and brittle; a few strokes with steel wool might help but it is not essential. After the board is clean cut it to proper size. Mark the dimensions and score the surface about 20/30 times with the blunt edge of the cutter on both sides; 

The cutting and sanding contaminates the board with dust and fine bits of copper, the handling of the boards deposits oil from your fingers. Before continuing I usually wipe the surface with alcohol. 


## Export the pcb as svg (2.5x, upper layer, board contours, multilayer, holes - black on white)

Once the pcb is done you need to export it:

## Open it with an image editing software to remove the white countour and leave only whats inside the board contours. Don't forget to mirror the circuit if you are using a one-sided copper clad, otherwise you can't solder the components

## save it as png or jpg
https://pixlr.com/it/

## convert from png/jpg back to svg
https://convertio.co/it/

## svg to stl
https://svg2stl.com/download/62ff87d2e13a861160a4098c

## mirror the stl vertically

## score the board once finished to remove unwanted connections