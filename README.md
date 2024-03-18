# SDRSharp-Cleanup-Plugin


A nice SDR# plugin for Short Wave, VHF, UHF listening enthusiasts, and...more!

The files in this zip archive add a novel denoising method like Sdrsharp's denoiser which provides spectral gating capability and defect-free denoising on shortwave, called cleanup. Cleanup is not limited to use with SDR#. https://github.com/falseywinchnet/Cleanup for more.
Cleanup is also present in sdrconsole since 3.3 as NR5.
This Plugin is compiled for SDR# 32bit, with .NET 8 (SDR# Studio release >= 1920).
<br>Note: The plugin has not been tested and will not work on unsupported/older version of SDR# Studio and SDR#.


#### Version: 1.0.6 - 03 17 2024
instructions for use:


As of 1.0.5, cleanup now performs estimation before any other denoisers(unless "after" enabled) and masks after them.
To use cleanup properly, follow this simple guide:

first, select the hann window and try to get about 3.2 or better bandwidth. 
If you can't, go narrower but get more than your speech + a little noise around it if possible.
Aim for 120% of what you actually need. For AM if you can't do this, use "full IQ" and try again.
For FM, this isn't necessary, just get 80% of the hill.
Use the built in notch filtering to notch out any strong carriers on SSB.

Secondly, tune cleanup. For AM and FM and very faint signals, turn squelch off.
Use the threshold to tune squelch. Use the comfort noise settings to tune it to just where there's very little noise.

Thirdly, turn cleanup off and tune any other denoisers. Tune them to minimize any attenuation.
the option "After" should be usually be enabled, but can be experimented with to refine results further.



**New Setup:**
<br>**1.** Unzip the file SDRSharp.Plugin.Cleanup.zip
<br>**2.** Copy the SDRSharp.Cleanup.dll file and cleanup.dll file file into the SDR# Studio "Plugins" default folder
<br>**3.** Alternate, should you prefer, create your own folder inside the default "Plugins" it could be "Cleanup", and copy there the dlls instead.
<br>>SDRSharp will load your plugin at next execution.


This plugin is provided for *free use for most cases* to the huge SDR# Studio users community.<br>

For comments: https://twitter.com/HFGCSSTREAMING
<br>Enjoy!

![Screenshot](https://github.com/falseywinchnet/PyITD/blob/main/screenshot.png)
