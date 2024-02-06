<h1 align="center"><img src="https://github.com/pizzaboxer/bloxstrap/raw/main/Images/Bloxstrap.png" width="28"/> Ultimate Fast Flags List</h1>

<h3 align="center">https://discord.gg/Q5JKyzuNRC</h3>

<h3 align="center">https://discord.gg/fastflags</h3>

##### Version: 5.0.0 [2/6/2024]
* **108 Currently Listed**
* **New Formatting**

 # How to use
* **Open the [Bloxstrap](https://github.com/pizzaboxer/bloxstrap) Menu**
* **Fast Flags >> Fast Flags Editor >> Import Json**
* **Paste in the JSON**
* **Then you should be good to go and save!**

###### Please just use bloxstrap its way easier

 # List Navigation
* **[Rendering](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#rendering)**
* **[Graphical](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#graphical-settings)**
* **[UI](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#user-interface)**
* **[Textures](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#textures)**
* **[Physics](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#physics)**
* **[Other FFlags](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#other-fflags)**
* **[Links](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#links)**

<img src="https://github.com/devstacking/Epic-Fast-Flags-List/assets/106433721/0d16e448-4097-44ef-9eef-c445155a4bcb" width="888"/>

### 

<h3 align="center">══════⊹⊱≼≽⊰⊹══════</h3>

<h1 align="center">Rendering API</h1>

### Metal
###### MacOS Only
```json
{ "FFlagDebugGraphicsPreferMetal": "True" }
```
### Vulkan
```json
{ "FFlagDebugGraphicsDisableDirect3D11": "True", "FFlagDebugGraphicsPreferVulkan": "True" }
```
### OpenGL
```json
{ "FFlagDebugGraphicsDisableDirect3D11": "True", "FFlagDebugGraphicsPreferOpenGL": "True" }
```
### DX10
```json
{ "FFlagDebugGraphicsPreferD3D11FL10": "True" }
```
### DX11
```json
{ "FFlagDebugGraphicsPreferD3D11": "True" }
```

<h1 align="center">Graphical Settings <sup>& other stuff</sup></h1>

### Smoother Terrain
```json
{ "FFlagDebugRenderingSetDeterministic": "True" }
```
### Heads
```json
{ "FFlagDebugLuaHeapDump": "True" }
```
### Graphics Quality Level
```json
{ "FIntRomarkStartWithGraphicQualityLevel": "1" }
```
### Low Quallity Terrain Textures
###### 4 for less quality 16, 32, 64 for higher quality
```json
{ "FIntTerrainArraySliceSize": "8" }
```
### Alternate Graphics Quality Selector
###### 1-21 bloxstrap preset
```json
{ "FFlagFixGraphicsQuality": "True" }
```
### Disable Shadows
```json
{ "FIntRenderShadowIntensity": "0" }
```
### Set Fps Limit
{ "DFIntTaskSchedulerTargetFps": "9999" }
```json
{ "DFIntTaskSchedulerTargetFps": "9999" }
```
### Enables Network Debug Tracker menu
##### Instructions: CTRL+F8
###### it's over.
```json
{ "DFFlagDebugEnableInterpolationVisualizer": "True" }
```
### Humanoid Outline
##### Draws an outline around every part and every humanoid
```json
{ "DFFlagDebugDrawBroadPhaseAABBs": "True" }
```
### Buggy ZPlane Camera *<sup>a.k.a xray</sup>*
```json
{ "DFFlagDebugDrawBroadPhaseAABBs": "0" }
```
### Preserve rendering quality with display setting
```json
{ "DFFlagDisableDPIScale": "True" }
```
### Low Graphics Quality w/ Max Render Distance
###### Explanation: 1-6 Are low graphics, Above 6 are high graphics. Like the 1-21 graphics slider
```json
{ "DFIntDebugFRMQualityLevelOverride": "1" }
```

<h4 align="center">FRM Levels</h4>

```
Low

1 = 3
2 = 2
3 = 6

High

4 = 7
5 = 11
6 = 14
7 = 15 
8 = 17
9 = 18
10 = 21
```

### Low Render Distance
###### [FRM](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#frm-levels)
```json
{ "DFIntDebugRestrictGCDistance": "1" }
```
### Disable Wind
```json
{ "FFlagGlobalWindRendering": "False", "FFlagGlobalWindActivated": "False" }
```
### Limits light updates
```json
{ "FIntRenderLocalLightUpdatesMax": "8", "FIntRenderLocalLightUpdatesMin": "6" }
```
### Disables fade in and fade out animation every light update
###### changes fade in ms!!
```json
{ "FIntRenderLocalLightFadeInMs": "0" }
```
### Makes avatars shiny 
###### [everything goes black on <3] ***[DFIntDebugFRMQualityLevelOverride is there to set your graphics to 10, You can change it to anything above 3: [Click here to view](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#frm-levels) ]***
```json
{ "DFIntRenderClampRoughnessMax": "-640000000", "DFIntDebugFRMQualityLevelOverride": "21" }
```
### Disable PostFX
```json
{ "FFlagDisablePostFx": "True" }
```
### Pause Voxelizer/Disable Baked Shadows
```json
{ "DFFlagDebugPauseVoxelizer": "True" }
```
### Gray Sky
```json
{ "FFlagDebugSkyGray": "True" }
```
### Disable Player Shadows
```json
{ "FIntRenderShadowIntensity": "0" }
```
### Force LOD on Meshes
```json
{ "DFIntCSGLevelOfDetailSwitchingDistance": "0", "FFlagGlobaDFIntCSGLevelOfDetailSwitchingDistanceL12lWindActivated": "0", "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0", "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0" }
```
### Lighting Attenuation
```json
{ "FFlagNewLightAttenuation": "True" }
```
### Enable GPULightCulling
###### Combine with [Lighting Attenuation](https://github.com/devstacking/Epic-Fast-Flags-List?tab=readme-ov-file#lighting-attenuation) for better vision
```json
{ "FFlagFastGPULightCulling3": "True" }
```
### Frame Buffer
###### Explnation: 0 makes white screen 1-3 makes other players have laggy movement, 4 is stable has better performance than 10 and less input lag
```json
{ "DFIntMaxFrameBufferSize": "4" }
```
### High Quality Textures 
###### *[1-3]*
```json
{ "DFFlagTextureQualityOverrideEnabled": "True", "DFIntTextureQualityOverride": "3", }
```
### Remove Grass
```json
{ "FIntFRMMinGrassDistance": "0", "FIntFRMMaxGrassDistance": "0", "FIntRenderGrassDetailStrands": "0", "FIntRenderGrassHeightScaler": "0" }
```
### Force MSAA 
###### *[0, 1, 2, 4, 8]*
```json
{ "FIntDebugForceMSAASamples": "4" }
```
### ShadowMap Bias 
###### ***[Future & ShadowMap]***
```json
{ "FIntRenderShadowmapBias": "75" }
```
<h1 align="center">User Interface</h1>

### New Report Menu
```json
{ "FStringReportAbuseMenuRoactForcedUserIds": "UserID" }
```

### Custom MicroProfile Scale
```json
{ "DFIntMicroProfilerDpiScaleOverride": "100" }
```

### V1 Menu
```json
{ "FIntNewInGameMenuPercentRollout3": "10000" }
```
### Hides gui
```json
{ "FFlagDebugAdornsDisabled": "True" }
```
### Dont Render UI
```json
{ "FFlagDebugDontRenderUI": "True" }
```
### Enable Audio Controller
```json
{ "FFlagTrackerLodControllerDebugUI": "True" }
```
### Disable Autocomplete
```json
{ "FFlagEnableCommandAutocomplete": "False" }
```
### Chrome UI TopBar
```json
{ "FFlagEnableInGameMenuChrome": "True" }
```
### Better Chrome UI TopBar
```json
{ "FFlagChromeBetaFeature": "True", "FFlagEnableChromePinnedChat": "True", "FFlagEnableInGameMenuChrome": "True", "FFlagEnableInGameMenuChromeABTest": "True", "FFlagEnableInGameMenuChromeSignalAPI": "True", "FFlagPlayerListChromePushdown": "True", "FFlagEnableChromeEscapeFix": "True", "FFlagEnableChromeMicShimmer": "True", "FFlagPlayerListChromePushdown": "True" }
```
### Chrome UI Topbar Removal
```json
{ "FFlagChromeBetaFeature": "False", "FFlagEnableChromePinnedChat": "False", "FFlagEnableInGameMenuChrome": "False", "FFlagEnableInGameMenuChromeABTest": "False", "FFlagEnableInGameMenuChromeSignalAPI": "False", "FFlagPlayerListChromePushdown": "False" }
```
### Disable Bubble Chat
```json
{ "FFlagEnableBubbleChatFromChatService": "False" }
}
```
### Disable Selfview
```json
{ "FFlagCoreGuiTypeSelfViewPresent": "False" }
```
### Remove VC Beta Badge
```json
{ "FFlagVoiceBetaBadge": "False", "FFlagTopBarUseNewBadge": "False", "FFlagEnableBetaBadgeLearnMore": "False", "FFlagBetaBadgeLearnMoreLinkFormview": "False", "FFlagControlBetaBadgeWithGuac": "False", "FStringVoiceBetaBadgeLearnMoreLink": "null" }
```
### Pin Chat on Chrome UI
```json
{ "FFlagEnableChromePinnedChat": "True" }
}
```
### Hide guis
###### ***Instructions: Replace "ID" with any group ID that you are in.***
```json
{ "DFIntCanHideGuiGroupId": "ID_HERE" }
```
### Disable Fullscreen Title Bar
```json
{ "FIntFullscreenTitleBarTriggerDelayMillis": "3600000" }
```
### Set Custom Font Size
```json
{ "FIntFontSizePadding": "1" }
```

<h1 align="center">Textures</h1>

### No Textures
```json
{
    "FStringPartTexturePackTable2022": "{\"glass\":{\"ids\":[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\"color\":[254,254,254,7]}}",
    "FStringPartTexturePackTablePre2022": "{\"glass\":{\"ids\":[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\"color\":[254,254,254,7]}}",
    "FStringTerrainMaterialTable2022": "",
    "FStringTerrainMaterialTablePre2022": ""
}
```
### Goofy Wood Textures
```json
{
    "FStringPartTexturePackTablePre2022": "{\"foil\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[238,238,238,255]},\"asphalt\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[227,227,228,234]},\"basalt\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[160,160,158,238]},\"brick\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[229,214,205,227]},\"cobblestone\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[218,219,219,243]},\"concrete\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[225,225,224,255]},\"crackedlava\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[76,79,81,156]},\"diamondplate\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[210,210,210,255]},\"fabric\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[221,221,221,255]},\"glacier\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[225,229,229,243]},\"glass\":{\"ids\":[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\"color\":[254,254,254,7]},\"granite\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[210,206,200,255]},\"grass\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[196,196,189,241]},\"ground\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[165,165,160,240]},\"ice\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[235,239,241,248]},\"leafygrass\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[182,178,175,234]},\"limestone\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[250,248,243,250]},\"marble\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[181,183,193,249]},\"metal\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[226,226,226,255]},\"mud\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[193,192,193,252]},\"pavement\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[218,218,219,236]},\"pebble\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[204,203,201,234]},\"plastic\":{\"ids\":[\"\",\"rbxassetid://9475422736\"],\"color\":[255,255,255,255]},\"rock\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[211,211,210,248]},\"corrodedmetal\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[206,177,163,180]},\"salt\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[249,249,249,255]},\"sand\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[218,216,210,240]},\"sandstone\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[241,234,230,246]},\"slate\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[235,234,235,254]},\"snow\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[239,240,240,255]},   \"credits\":{\"ids\":[\"pastelist/on/discord\",\"https://kits.ju.mp\"],\"color\":[238,238,238,255]},   \"wood\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[217,209,208,255]},\"woodplanks\":{\"ids\":[\"rbxassetid://15474524700\",\"rbxassetid://452400917\"],\"color\":[207,208,206,254]}}"
}
```
### Troll Face Textures
```json
{
    "FStringPartTexturePackTable2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[238,238,238,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[227,227,228,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[160,160,158,238]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[229,214,205,227]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,219,219,243]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,225,224,255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[76,79,81,156]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,210,210,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[221,221,221,255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,229,229,243]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873284556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,206,200,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[196,196,189,241]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[165,165,160,240]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,239,241,248]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[182,178,175,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[250,248,243,250]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[181,183,193,249]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[226,226,226,255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[193,192,193,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,218,219,236]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[204,203,201,234]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://9475422736\u0022],\u0022color\u0022:[255,255,255,255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[211,211,210,248]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[206,177,163,180]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[249,249,249,255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,216,210,240]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[241,234,230,246]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,234,235,254]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[239,240,240,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[217,209,208,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[207,208,206,254]}}",
    "FStringPartTexturePackTablePre2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[238,238,238,255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[227,227,228,234]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[160,160,158,238]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[229,214,205,227]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,219,219,243]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,225,224,255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[76,79,81,156]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,210,210,255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[221,221,221,255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[225,229,229,243]},\u0022glass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://9873284556\u0022,\u0022rbxassetid://9438453972\u0022],\u0022color\u0022:[254,254,254,7]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[210,206,200,255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[196,196,189,241]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[165,165,160,240]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,239,241,248]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[182,178,175,234]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[250,248,243,250]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[181,183,193,249]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[226,226,226,255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[193,192,193,252]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,218,219,236]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[204,203,201,234]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://9475422736\u0022],\u0022color\u0022:[255,255,255,255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[211,211,210,248]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[206,177,163,180]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[249,249,249,255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[218,216,210,240]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[241,234,230,246]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[235,234,235,254]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[239,240,240,255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[217,209,208,255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://15482832278\u0022,\u0022rbxassetid://14983259444\u0022],\u0022color\u0022:[207,208,206,254]}}"
}
```
### Black Textures
```json
{
    "FStringPartTexturePackTable2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glass\u0022:{\u0022ids\u0022:[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\u0022color\u0022:[55, 55, 55, 255]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022plastic\u0022:{\u0022ids\u0022:[\u0022\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]}}",
    "FStringPartTexturePackTablePre2022": "{\u0022foil\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022brick\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022cobblestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022concrete\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022diamondplate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022fabric\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glass\u0022:{\u0022ids\u0022:[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\u0022color\u0022:[55, 55, 55, 255]},\u0022granite\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022grass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ice\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022marble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022metal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pebble\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022corrodedmetal\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sand\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022slate\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022wood\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022woodplanks\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022asphalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022basalt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022crackedlava\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022glacier\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022ground\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022leafygrass\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022limestone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022mud\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022pavement\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022rock\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022salt\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022sandstone\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]},\u0022snow\u0022:{\u0022ids\u0022:[\u0022rbxassetid://0\u0022,\u0022rbxassetid://0\u0022],\u0022color\u0022:[55, 55, 55, 255]}}"
}
```
### Minecraft Textures
```json
{
	"FStringPartTexturePackTablePre2022": "{\"foil\":{\"ids\":[\"rbxassetid://9873266399\",\"rbxassetid://9438410239\"],\"color\":[238,238,238,255]},\"asphalt\":{\"ids\":[\"rbxassetid://9867974823\",\"rbxassetid://9844502433\"],\"color\":[227,227,228,234]},\"basalt\":{\"ids\":[\"rbxassetid://11545552824\",\"rbxassetid://11545440462\"],\"color\":[160,160,158,238]},\"brick\":{\"ids\":[\"rbxassetid://9924770651\",\"rbxassetid://9924770538\"],\"color\":[229,214,205,227]},\"cobblestone\":{\"ids\":[\"rbxassetid://9919719550\",\"rbxassetid://9438453972\"],\"color\":[218,219,219,243]},\"concrete\":{\"ids\":[\"rbxassetid://9924775913\",\"rbxassetid://9924775826\"],\"color\":[225,225,224,255]},\"crackedlava\":{\"ids\":[\"rbxassetid://9920485426\",\"rbxassetid://9438453972\"],\"color\":[76,79,81,156]},\"diamondplate\":{\"ids\":[\"rbxassetid://10237721036\",\"rbxassetid://9438453972\"],\"color\":[210,210,210,255]},\"fabric\":{\"ids\":[\"rbxassetid://9920517963\",\"rbxassetid://9438453972\"],\"color\":[221,221,221,255]},\"glacier\":{\"ids\":[\"rbxassetid://9920518995\",\"rbxassetid://9438453972\"],\"color\":[225,229,229,243]},\"glass\":{\"ids\":[\"rbxassetid://9873284556\",\"rbxassetid://9438453972\"],\"color\":[254,254,254,7]},\"granite\":{\"ids\":[\"rbxassetid://9920550720\",\"rbxassetid://9438453972\"],\"color\":[210,206,200,255]},\"grass\":{\"ids\":[\"rbxassetid://11152995545\",\"rbxassetid://9267183930\"],\"color\":[196,196,189,241]},\"ground\":{\"ids\":[\"rbxassetid://11546360009\",\"rbxassetid://11545533676\"],\"color\":[165,165,160,240]},\"ice\":{\"ids\":[\"rbxassetid://9920556429\",\"rbxassetid://9438453972\"],\"color\":[235,239,241,248]},\"leafygrass\":{\"ids\":[\"rbxassetid://11152995545\",\"rbxassetid://9267183930\"],\"color\":[182,178,175,234]},\"limestone\":{\"ids\":[\"rbxassetid://9920561624\",\"rbxassetid://9438453972\"],\"color\":[250,248,243,250]},\"marble\":{\"ids\":[\"rbxassetid://9873292869\",\"rbxassetid://9438453972\"],\"color\":[181,183,193,249]},\"metal\":{\"ids\":[\"rbxassetid://11546526557\",\"rbxassetid://11546431794\"],\"color\":[226,226,226,255]},\"mud\":{\"ids\":[\"rbxassetid://9920578676\",\"rbxassetid://9438453972\"],\"color\":[193,192,193,252]},\"pavement\":{\"ids\":[\"rbxassetid://11546539560\",\"rbxassetid://11546440685\"],\"color\":[218,218,219,236]},\"pebble\":{\"ids\":[\"rbxassetid://9920581197\",\"rbxassetid://9438453972\"],\"color\":[204,203,201,234]},\"plastic\":{\"ids\":[\"\",\"rbxassetid://9868015012\"],\"color\":[255,255,255,255]},\"rock\":{\"ids\":[\"rbxassetid://11546570730\",\"rbxassetid://11546456858\"],\"color\":[211,211,210,248]},\"corrodedmetal\":{\"ids\":[\"rbxassetid://11545623165\",\"rbxassetid://11545476330\"],\"color\":[206,177,163,180]},\"salt\":{\"ids\":[\"rbxassetid://9920590478\",\"rbxassetid://9438453972\"],\"color\":[249,249,249,255]},\"sand\":{\"ids\":[\"rbxassetid://11546588111\",\"rbxassetid://11546468464\"],\"color\":[218,216,210,240]},\"sandstone\":{\"ids\":[\"rbxassetid://9920596353\",\"rbxassetid://9438453972\"],\"color\":[241,234,230,246]},\"slate\":{\"ids\":[\"rbxassetid://9867974823\",\"rbxassetid://9844502433\"],\"color\":[235,234,235,254]},\"snow\":{\"ids\":[\"rbxassetid://11536062048\",\"rbxassetid://11108916253\"],\"color\":[239,240,240,255]},\"wood\":{\"ids\":[\"rbxassetid://9867974813\",\"rbxassetid://9844454989\"],\"color\":[217,209,208,255]},\"woodplanks\":{\"ids\":[\"rbxassetid://9867974813\",\"rbxassetid://9844454989\"],\"color\":[207,208,206,254]}}"
}
```

<h1 align="center">Physics</h1>

### Stick unanchored parts to you
###### - = up, + = down
###### blame popbob he said it was ok to leak this
```json
{ "DFIntSolidFloorPercentForceApplication": "-1000", "DFIntNonSolidFloorPercentForceApplication": "-5000" }
```
### Breaks glitches stuff
###### All type of wallhops, longjumps, headhitters and probably more stop working
```json
{ "DFFlagSimHumanoidPhysics": "True" }
```
### Max Raycast Distance
###### Break legs collision from 2 to -inf, kinda break camera on values over 3
###### noclip cam on 3
```json
{ "DFIntRaycastMaxDistance": "3" }
```
### Possible Super Jump
###### i thought this was patched thats why i removed it lol
```json
{ "DFIntNewRunningBaseGravityReductionFactorHundredth": "1500" }
```
### Breaks movement on higher negative values
```json
{ "FIntPGSAngularDampingPermilPersecond": "-10000" }
```
### it does something to movement cant describe rn cus im busy
```json
{ "FIntPGSAngularDampingPermilPersecond": "0" }
```
### It allows you to fall quicker and ignore certain block designs
```json
{ "FFlagHumanoidOnlySetCollisionsOnStateChangeDefaultIsEnabled": "False", "FFlagHumanoidParallelFasterSetCollision": "True" }
```
### Gear Desync
###### a.k.a dos not let you load games
```json
{ "DFIntDataSenderRate": "-1" }
```
### Freezes character in any state, can cause crashes, basically stacks input data
```json
{ "FFlagSimIslandizerManager": "False" }
```
### Fake Lag
```json
{ "DFIntS2PhysicsSenderRate": "1" }
```
### ultiamt desync flag!! 😱😱😱
```json
{ "DFIntS2PhysicsSenderRate": "1", "FIntPGSAngularDampingPermilPersecond": "0" }
```
### Noclip 1
###### adjust the value so u dont fall through the ground
```json
{ "DFFlagAssemblyExtentsExpansionStudHundredth": "-50" }
```
### Noclip 2
```json
{
{ "FIntPGSPenetrationMarginMax": "2147483647", "FIntPGSPenetrationMarginMin": "2147483647" }
}
```
### Noclip Combo
###### adjust the value so u dont fall through the ground
```json
{ "FIntPGSPenetrationMarginMax": "2147483647", "FIntPGSPenetrationMarginMin": "2147483647", "DFFlagAssemblyExtentsExpansionStudHundredth": "-50" }
```
### Teleportation
###### a.k.a control the unanchored
```json
{ "FIntPGSPenetrationMarginMax": "-100000000", "FIntPGSPenetrationMarginMin": "-100000000" }
```
### limited speed fflag that works only in a few games
###### one of them being Phantom Forces, and it makes you only slightly faster
```json
{ "DFIntDebugSimPhysicsSteppingMethodOverride": "10000000" }
```
### Hip Height
###### Very controllable bounce, only works with negative values, 0 allows you to hover
```json
{ "DFIntMaxAltitudePDStickHipHeightPercent": "-200" }
```
### Noclip <sup>literally</sup>
```json
{ "DFIntSHCellMinSizeAsBitShift": "4" }
```
### Wallglide
```json
{ "DFFlagUnstickForceAttackInTenths": "-4" }
```

<h1 align="center">other fflags</h1>

### Disable ADs
```json
{ "FFlagAdServiceEnabled": "False" }
```

### Disable Telemetry 
###### *[This doesn't fully disable telemetry]*
```json
{ "FFlagDebugDisableTelemetryEphemeralCounter": "True", "FFlagDebugDisableTelemetryEphemeralStat": "True", "FFlagDebugDisableTelemetryEventIngest": "True", "FFlagDebugDisableTelemetryPoint": "True", "FFlagDebugDisableTelemetryV2Counter": "True", "FFlagDebugDisableTelemetryV2Event": "True", "FFlagDebugDisableTelemetryV2Stat": "True" }
```
### Scroll Speed
```json
{ "FIntScrollWheelDeltaAmount": "140" }
```
### Surf the web inside of Roblox
###### Click the Beta badge or the 13+ badge to open the webview browser.
```json
{ "FFlagTopBarUseNewBadge": "True", "FStringTopBarBadgeLearnMoreLink": "https://google.com/", "FStringVoiceBetaBadgeLearnMoreLink": "https://google.com/" }
```
### Sounds use physical velocity and become distorted
```json
{ "FFlagSoundsUsePhysicalVelocity": "True" }
```
### Shows the state of a flag
```json
{ "FStringDebugShowFlagState": "FLAG_HERE" }
```
###### e.g
```json
{ "FStringDebugShowFlagState": "DFIntTaskSchedulerTargetFps, ChannelName" }
```
### MTU 
###### ***[Might Improve Ping]***
```json
{ "DFIntConnectionMTUSize": "MTU_HERE" }
```
### No Internet Disconnect 
###### *[You will still be kicked but the message wont show.]*
```json
{ "DFFlagDebugDisableTimeoutDisconnect": "True" }
```
### Quick Game Launch 
###### *[BUGGY]*
```json
{ "FFlagEnableQuickGameLaunch": "True" }
```
### Allows you to change voice chat distance 
###### default: [Min 7 Max 80]
```json
{ "DFIntVoiceChatRollOffMinDistance": "7", "DFIntVoiceChatRollOffMaxDistance": "80" }
```
### Disable In-Game Purchases
```json
{ "DFFlagOrder66": "True" }
```
### Disable Chat
```json
{ "FFlagDebugForceChatDisabled": "True" }
```
### Limit audios that are being played
```json
{ "DFIntMaxLoadableAudioChannelCount": "1" }
```
### Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's a non-functioning UI too. Also adds a blue circle to your humanoid.
```json
{
	"FFlagDebugHumanoidRendering": "True"
}
```
### Custom Disconnect Message
```json
{
	"FFlagReconnectDisabled": "True",
	"FStringReconnectDisabledReason": "You're stupid and I hate you"
}
```
### Display FPS
```json
{
	"FFlagDebugDisplayFPS": "True"
}
```
### Verified Badge
```json
{
	"FStringWhitelistVerifiedUserId": "UserID"
}
```
### Verified Badge on everyone
```json
{
	"FFlagOverridePlayerVerifiedBadge": "True"
}
```
### Applies cool colors to Unthemed Stuff
```json
{
	"FFlagDebugDisplayUnthemedInstances": "True"
}
```
### Show Outlined Chunks
```json
{
	"FFlagDebugLightGridShowChunks": "True"
}
```
### Remove Disconnect Blur/Loading Blur
```json
{
	"FIntRobloxGuiBlurIntensity": "0"
}
```
### Disable Dynamic Heads Animations
```json
{
	"DFFlagEnableDynamicHeadByDefault": "False"
}
```
### failsafehumanoid
```json
{
	"FFlagFailsafeHumanoid_3": "True"
}
```
### Automatically unmutes your mic on join
```json
{
	"FFlagDebugDefaultChannelStartMuted": "False"
}
```
### Overlay that shows what you type 
```json
{
	"FFlagDebugTextBoxServiceShowOverlay": "True"
}
```
### ~~Disable Output Device~~
### opt-out Experience Language
###### Removes the Experience Language option in settings
```json
{
	"FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Exclusive Fullscreen
###### Alt + Delete
```json
{
	"FFlagHandleAltEnterFullscreenManually": "False"
}
```
### Lets you change the zoom out limit
###### infinite zoom out!!
```json
{
	"FIntCameraMaxZoomDistance": "9999"
}
```
### Limits number of animations being played
```json
{
	"DFIntMaxActiveAnimationTracks": "0"
}
```
### Limits Logs History
```json
{
	"DFIntMaxLogHistory": "1"
}
```

### Prevents Remote Events from running
###### W SPECTRO
```json
{
	"DFIntRemoteEventSingleInvocationSizeLimit": "1"
}
```

<h1 align="center">Links</h1>

### [Make Your Own Custom Roblox Textures](https://github.com/GoingCrazyDude/roblox-custom-textures/blob/main/README.md) *[Github Repo Link]*
### [MEGA FLAG LIST](https://discord.com/channels/1099468797410283540/1139962301991104582/1170417533355036712) *[Bloxstrap Server]*
### [Bloxstrap](https://github.com/pizzaboxer/bloxstrap) *[Github Repo Link]*
### [NVIDIA Shaders Guide](https://github.com/catb0x/Roblox-Shaders-Guide) *[Github Repo Link]*
### [EnableAnselForRoblox](https://github.com/DED0026/EnableAnselForRoblox) *[Github Repo Link]*
### [potato fflags](https://github.com/catb0x/Roblox-Potato-FFlags) *[Github Repo Link]*
### [Fake Roblox Player Internal Patcher](https://github.com/devstacking/Roblox-Player-Internal-Patcher/releases/download/Release/FakeInternal.exe) *[Download Link]*

### Patched in 0, 608, 1, 6080485
```
DFIntFreeFallBalanceP 
DFIntFreeFallOrientationP
DFIntGettingUpBalanceD
DFIntGettingUpBalanceP
DFIntLandedBalanceD
DFIntLandedBalanceP
DFIntNewRunningBaseAltitudeD
DFIntNewRunningBaseAltitudeP
DFIntRunningBaseAltitudeD
DFIntRunningBaseAltitudeP
DFIntRunningBaseOrientationP
FFlagDebugSimIntegrationStabilityTesting
```

<h4 align="center">‧⁺̣˚̣̣*̣̩⋆̩·̩̩୨˚̣̣̣̣͙୧·̩̩⋆̩*̣̩˚̣̣⁺̣‧ You've reached the bottom of the list! ‧⁺̣˚̣̣*̣̩⋆̩·̩̩୨˚̣̣̣̣͙୧·̩̩⋆̩*̣̩˚̣̣⁺̣‧୨</h4>

# List Information
* Creation Date: 9:46 PM 08/25/2023 
* Github Publish Date: 12/26/2023
###### [<sup>OG</sup>](https://rentry.org/uffl/)

<h3 align="center">FastFlags 2024®<sup>eal</sup></h3>
