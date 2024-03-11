# SDRSharp-Cleanup-Plugin


A nice SDR# plugin for Short Wave listening enthusiasts, and...more!

#### NOTE
I forgot to make this abundantly clear.
DO NOT USE the other denoisers if you value the squelch. Only use a hanning window if you value the squelch.
The squelch will NOT WORK correctly when less than 1200hz of bandwidth are considered.
The more uniform, correct, and wideband the noise you provide(by setting your filter wider,within reason, maybe 120% of the BW you want)
the better the squelch will work. The squelch does not at this time work in AM mode, only SSB modes.
The squelch feature also provides some reduction of cpu usage.

also, we recommend a 16 bit sdr with a 16 bit output only- no forced 8bit mode 

# Version: 1.0 - 11 Jan 2024 


The files in this zip archive add a novel denoising method like Sdrsharp's denoiser which provides spectral gating capability and defect-free denoising on shortwave, called cleanup. Cleanup is not limited to use with SDR#. https://github.com/falseywinchnet/Cleanup for more.
<br>Not limited to VLF-HF! It can be used at any SDR# available frequency, but for wideband, we recommend sdrsharp's other denoisers.
This Plugin is compiled for SDR# 32bit, with .NET 8 (SDR# Studio release >= 1920).
<br>Note: The plugin has not been tested and will not work on unsupported/older version of SDR# Studio and SDR#.


**New Setup:**
<br>**1.** Unzip the file SDRSharp.Plugin.Cleanup.zip
<br>**2.** Copy the SDRSharp.Cleanup.dll file and cleanup.dll file file into the SDR# Studio "Plugins" default folder
<br>**3.** Alternate, should you prefer, create your own folder inside the default "Plugins" it could be "Cleanup", and copy there the dlls instead.
<br>>SDRSharp will load your plugin at next execution.


This plugin is provided for *free use for most cases* to the huge SDR# Studio users community.<br>

For comments: https://twitter.com/HFGCSSTREAMING
<br>Enjoy!

![Screenshot](https://github.com/falseywinchnet/PyITD/blob/main/screenshot.png)
