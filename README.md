
![HSSSSforVR](https://github.com/arthurOmanko/HSSSSforVR/assets/68005887/6bcae923-5174-46b0-b3c2-d645dbfddb54)

# HoneySelect HSSSS on VR mod
This experimantal mod is for applying HSSSS.dll (already existing HoneySelect Subsurface Scattering(SSS) Shader mod) on VR.
If User wants to know about Subsurface Scattering in detail, please see the below,

- About Subsurface scattering
https://en.wikipedia.org/wiki/Subsurface_scattering


## [Installation]
1. Extract the zip file into User's HoneySelect directory.
2. Run HoneySelect_(64|32).exe or StudioNEO_(64|32).exe with --vr option (when having VRmod and being able to use on HoneySelect or StudioNEO)
3. Enjoy super high quality on VR!

**Caution!** 
- This mod is currently able to be used on StudioNEO and MainGame+CharaMake.
  Or By different version of HSSSS.dll and HSSSSforVR.dll, this might maybe not be able to get used properly.
- On HSSSS config menu, especially, [Normal Blur Iterations] value must be smaller on VR, 
  otherwise FPS on VR will get much decreased.
- Alpha value of backlight would influence looks of charas largely.
  If so, please set alpha value of backlight at 0.
- If [AmbientOcclusion], [GlobalIllumination] or [PCSS] enabled on HSSSS config in VR scene and having heavy setting, FPS on VR might be much decreased.
  Then recondiser to make them lighter or off.


## [Requirements]
- Game updated with the last patch and DLC installed
- Installed and set up SteamVR
- VRmod (VRGIN.dll)
- HSExtSave.dll
- HoneySelect Subsurface Scattering(SSS) Shader mod (HSSSS.dll)
  version 1.7.0 (or more (presently not guaranteed))


## [Usage]
- Same as HSSSS.dll

## [Uninstall]
Please remove HSSSSforVR.dll in (${GameFolder}\Plugins). Or when you remove/uninstall HSSSS.dll, please also remove HSSSSforVR.dll at same time.

## Settings & Tweaks
Settings can be changed in the file *UserData/modprefs.ini*, of which HSSSSforVR setting tag is added the first time you start the game.  
Tag      | Default | Effect |
----     | ------  | ------ |
`<NormalBlurIterationAlwaysSetAt0>` | 1 | In order to avoid decreased FPS,  [Normal Blur Iterations] value of HSSSS on VR is set at 0 whenever game starting, scene loading.
`<backDirectionalLightAlphaAlwaysSetAt0>` | 1 | In order to improve looks of charas, alpha value of backlight is set at 0 always on VR.
