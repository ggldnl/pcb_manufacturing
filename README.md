# PCB manufacturing

This is a simple guide (and a reference for me in the future) to make simple PCBs at home. Other than the actual materials used for the synthesis, a resin printer is required.

# BOM

|Item   |Store   |
|---|---|
|Single sided copper clad boards   |[link](https://www.amazon.it/gp/product/B07RBK9WW6/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1)   |
|Photosensitive film   |[link](https://www.amazon.it/gp/product/B07YG6GY8M/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&psc=1)   |
|Ferric Chloride   |   |
|Sodium Carbonate (soda ash or washing soda)   |   |
|Acetone   |   |

# Tools

- Resin printer
- Drill press (strongly recommended but you can even do it by hand with bad results)
- Scoring board
- Ruler
- Cutter

# Convert the PCB to a printable file

For this guide I will refer to [easyEDA](https://easyeda.com/).

forgive me if the screens are in Italian

### 1. File > Export > SVG...

The export menu will show up

![Step 1 screenshot](https://images.tango.us/public/screenshot_df9e03b0-75f2-4808-8ee1-06d5db583f7b.png?crop=focalpoint&fit=crop&fp-x=0.2119&fp-y=0.1962&fp-z=2.5464&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 2. Drag the dropdown menu and select "2.5x", leave the other settings as shown in the image
![Step 2 screenshot](https://images.tango.us/public/screenshot_42eafd24-0fbd-49d7-b45e-3494b90e746e.png?crop=focalpoint&fit=crop&fp-x=0.4986&fp-y=0.2754&fp-z=2.7907&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 3. Uncheck "Bottom Silk Layer"
![Step 3 screenshot](https://images.tango.us/public/screenshot_0c659db6-ba1a-4152-bcea-8ad28828ce19.png?crop=focalpoint&fit=crop&fp-x=0.4872&fp-y=0.4607&fp-z=3.1866&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 4. Click on "Export"
![Step 4 screenshot](https://images.tango.us/public/screenshot_d7f4df41-a1a6-4ee9-a3e8-b1214f5b4e57.png?crop=focalpoint&fit=crop&fp-x=0.5531&fp-y=0.7885&fp-z=3.0094&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)

__Source:__ [Tango](https://app.tango.us/app/workflow/48a8c24c-b20f-4d17-b053-4a210ef0bb6e?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)

## Edit the generated SVG

I generally use [pixlr](https://pixlr.com/us/e/#editor) but any editor (both online or offline) will suffice. Don't mind the PCB I used, this is just for reference.

### 1. Use the magic wand selection tool
![Step 1 screenshot](https://images.tango.us/public/screenshot_e0662550-d70b-409c-9612-ea39befc112d.png?crop=focalpoint&fit=crop&fp-x=0.0276&fp-y=0.1477&fp-z=3.0923&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 2. Select the white countour outside the board outlines
easyEDA automatically pad the SVGs. We need to remove the padding in order to scale the STL that we are about to make to proper size
![Step 2 screenshot](https://images.tango.us/public/edited_image_b7c49f94-8e8e-453b-a8a6-0219b18c024d.png?crop=focalpoint&fit=crop&fp-x=0.3697&fp-y=0.5341&fp-z=2.0000&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 3. Selection > Invert selection…
![Step 3 screenshot](https://images.tango.us/public/screenshot_4c7c4915-a0d4-4f5b-b127-3efb0c98e951.png?crop=focalpoint&fit=crop&fp-x=0.2109&fp-y=0.1690&fp-z=2.3587&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 4. Cut the selection


### 5. File > New iamge..…
![Step 5 screenshot](https://images.tango.us/public/screenshot_b8b490e4-9fc4-4b99-a8f1-2e79edc9dac1.png?crop=focalpoint&fit=crop&fp-x=0.2002&fp-y=0.1839&fp-z=2.3587&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 6. Click on "clipboard…"
This will create a new image the size of the selected item
![Step 6 screenshot](https://images.tango.us/public/screenshot_14de7ecd-cad9-44dd-9cce-b8195dfb67dc.png?crop=focalpoint&fit=crop&fp-x=0.2284&fp-y=0.3454&fp-z=2.3391&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 7. Click on "Create"
![Step 7 screenshot](https://images.tango.us/public/screenshot_56d8455c-2364-4c27-a2b2-e20af457b24d.png?crop=focalpoint&fit=crop&fp-x=0.7760&fp-y=0.8092&fp-z=3.9588&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 8. Paste the selection
![Step 8 screenshot](https://images.tango.us/public/screenshot_ae89797e-df25-49e0-8217-e0e05f8a23bf.png?crop=focalpoint&fit=crop&fp-x=0.3658&fp-y=0.5526&fp-z=2.8696&w=1200&mark-w=0.2&mark-pad=0&mark64=aHR0cHM6Ly9pbWFnZXMudGFuZ28udXMvc3RhdGljL21hZGUtd2l0aC10YW5nby13YXRlcm1hcmsucG5n&ar=1920%3A941)


### 9. File > Export as SVG...

Now you have an SVG cut to proper size without padding.

__Source:__ [Tango](https://app.tango.us/app/workflow/dfbabeed-db44-41a0-be2a-5b671c5a0cbb?utm_source=markdown&utm_medium=markdown&utm_campaign=workflow%20export%20links)


## Convert to SVG to STL

For this task I use [this online tool](https://svg2stl.com/) but this often does not yield good results and post processing of the STL file is required (often in [tinkercad](https://www.tinkercad.com/)).
I'll try to write a script to generate an STL file starting from a PNG/SVG (since all the PNGs we will use are b/w).

## Slice the STL

Drop the file in your favourite slicer. I use [lychee slicer](https://mango3d.io/lychee-slicer-3-for-sla-3d-printers/). 
Rescale the file to match the size of the copper clad board. 
Mirror the STL vertically (big side on x axis), otherwise you will not be able to solder the components on it. When selecting the resin, adjust the exposure of the first layer to 18 seconds and the exposure for the other layers to 0; I found that this works pretty well for me, fine tune the first layer exposure time to suit your needs. 


# Prepare the board

The first thing to do is clean the card. I usually rub the copper clad board with fine grain sanding paper (320-400 grit) to even the surface and remove the stains; do not overdo it because the copper film is thin and could wear out too much, making the traces too thin and brittle; a few strokes with steel wool might help but it is not essential. After the board is clean cut it to proper size. Mark the dimensions and score the surface about 20/30 times with the blunt edge of the cutter on both sides; 

The cutting and sanding contaminates the board with dust and fine bits of copper, the handling of the boards deposits oil from your fingers. Before continuing I usually wipe the surface with alcohol.


# Apply the photosensitive film

TODO: need images

# Burn the traces on the copper clad board with the photosensitive film on

TODO: need images

# Develop the traces

TODO: need images

# Etch the PCB

TODO: need images

# Rinse in acetone

TODO: need images

# Board post processing

Check all the traces with a multimeter and score the board with the currer to remove unwanted connections.