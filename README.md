# True IR Metering with Reveni Labs SPOT METER mk1 and  mk2

The Reveni Labs Spot Meters mk1 and mk2 are great tools, but they natively had infrared sensitivity.

This was fixed in the v1.8 firmware update (but the v1.9 firmware will give the option to chose between visible, visible+ir, ir). 
This fix is possible because the device actually uses two sensors: one for visible light + IR, and another strictly for IR cancellation. Meanwhile, the mk3 directly uses an IR-cut glass to prevent IR sensitivity altogether.
The meter need to be in "visible+ir" (for v1.9+ on MK2).

<img width="200" alt="image" src="https://github.com/user-attachments/assets/fdfe7a9d-03ed-4469-9b08-3e15ce03cd13" />  
(only CH1 chanel where used before v1.8 and then CH1 is used to cancel ir from v1.8) 

Special thanks to Matt from Reveni Labs for the info!

Because of this extended IR sensitivity, the meter can be used to meter infrared film simply by placing an IR-pass filter directly in front of the meter's sensor, letting only IR light reach the meter's sensor.

Because the meter relies on a binocular aiming principle (you keep both eyes open so your brain merges the meter's internal display with your real-world vision), you can clearly see what you are aiming at without being blinded by the filter.

I ran some bracketing tests to find an "IR-filtered ISO" for spot metering (feel free to do your own bracketing to match your development routine). This allows you to choose an ISO depending on how white you want the foliage to appear. You just aim at the foliage with the filter in front of the meter and get your exposure! There is no need to bracket or randomly overexpose +10EV compared to using a regular meter.

I tested the only two infrared films readily available on the market: Ilford SFX and Agfa Aviphot 200 (aka Rollei Infrared, Retro 400s, Superpan 200). Since all these Rollei stocks are the exact same film, I decided to test and develop them at different speeds (push/pull): 100, 200, and 400 ISO.

For the filter, I used the Neewer IR720.

Special thanks to u/Kareem-Abdul-Jabroni for giving me these films to test!

## Results

To use the calibration "chart", simply choose the image that matches your film (stock and push/pull for the Aviphot). Then, choose the brightness you want for the subject you are metering, and set your meter to the ISO specified on top of that specific example. Finally, meter your subject with the IR-pass filter in front of the meter, put the filter back on your camera lens, and shoot with the parameters shown on the meter.

!! For development, if you use Rodinal, you can just use the times, dilutions, and temperatures I specified on all 4 tests. But if you want to use another developer, ONLY use the results for Aviphot @200 and @400 (I don't trust the times I found for Aviphot @100 and SFX @200 to match those speeds, I believe the time for Aviphot @100 is too long and the time for SFX is too short). !!!


<img width="5600" height="941" alt="it_spot_SFX+Neewer IR720_v2" src="https://github.com/user-attachments/assets/db4c6e9c-1c34-449d-83c9-a7c48da5075d" />

<img width="5600" height="941" alt="ir_spot_AVIPOT200_@100+Neewer IR720_v2" src="https://github.com/user-attachments/assets/d8dafaf5-b5a0-419e-b7c6-e3bda5af135e" />

<img width="5600" height="941" alt="ir_spot_AVIPOT200_@200+Neewer IR720_v2" src="https://github.com/user-attachments/assets/86bd6cb8-5c0a-4654-9284-41f4af08c708" />

<img width="5600" height="941" alt="ir_spot_AVIPOT200_@400+Neewer IR720_v2" src="https://github.com/user-attachments/assets/94072b1a-c81f-434b-9e92-a4deeab54136" />

## Example

This shot was taken using Rollei Infrared developed at 400 ISO. I shot it at 6 ISO and aimed the meter directly at the tree.

<img width="4765" height="3180" alt="_DSC4840" src="https://github.com/user-attachments/assets/5110a979-edfc-4b98-9011-26ebd2591173" />

## Technical Details

### Development Times

I used Rodinal 1+50 at 20°C with agitation every 2 mins for everything.

For the times, I compared what I found on the Massive Dev Chart and settled on:

* **SFX @200:** 10 min
* **Aviphot @100:** 15 min
* **Aviphot @200:** 17 min
* **Aviphot @400:** 22 min

However, times on the Massive Dev Chart are not always very accurate and can be quite random, especially for films that only have a single entry. Developing with another developer at these specified ISOs might not yield the exact same results(the aviphot @100 time is too high i think), but for Aviphot at 200 and 400 ISO, it should be fine with other dev.

Here are the different times I found on the chart, on the back of my Rodinal bottle, and on the datasheets for these films at 1+50 20°C. I excluded times that already compensated for the filter effect:

* **SFX @200:** 10 min
* **Aviphot @100:** 15 min
* **Aviphot @200:** 17 min, 9 min (1+43), 17 min (box)
* **Aviphot @400:** 22 min, 22 min (box)

### The Shooting

For the shooting, I used my Nikon F3 with a Makinon 28mm f/2.8 lens set at f/4 with a Neewer 720nm filter, and I chose a sunny, cloudless day.

I metered with the filter in front of the spot meter, aiming at dense and uniformly lit vegetation, and wrote everything down in a notebook while shooting. I shot 7 exposures for each film, then rewound the spool.

### Development Process

For the development, I cut the films to load just the 7 exposures into the tank, saving the rest of the rolls for later.

I filled a large bucket with water, cooled it with ice until it reached 20°C, and added ice during the process if the temperature rose, keeping it within +/- 1°C.

I agitated the tank every 2 minutes.

### Scanning

I used a Sony A7II for scanning, exposing to get the film base just before clipping, and kept this same exposure for the entire strip.

I imported the files into Lightroom Classic, set the white balance, and used the color picker on the film base and leader in the tone curve. I inverted the curve using these two points and synced these exact parameters across every frame of the roll without any further adjustments.








do to:
- redo sfx+ aviphot @100 and find the good dev time

