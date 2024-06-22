
![image](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/1600b235-52b6-479c-a468-d1d3197d2f0e/deqjnrb-fe2fd641-f4c8-4612-91e7-162786e724a8.png/v1/fill/w_1280,h_720,q_80,strp/kreedz_wallpaper__kz_bhop_lucid__by_nyu_one_deqjnrb-fullview.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9NzIwIiwicGF0aCI6IlwvZlwvMTYwMGIyMzUtNTJiNi00NzljLWE0NjgtZDFkMzE5N2QyZjBlXC9kZXFqbnJiLWZlMmZkNjQxLWY0YzgtNDYxMi05MWU3LTE2Mjc4NmU3MjRhOC5wbmciLCJ3aWR0aCI6Ijw9MTI4MCJ9XV0sImF1ZCI6WyJ1cm46c2VydmljZTppbWFnZS5vcGVyYXRpb25zIl19.3acDxrOua8fplh0u3JvhWKlkUBcRtEBY4eAdc27G2f4)

###### Image by [Nyu-One](https://www.deviantart.com/nyu-one) under [CC BY-NC-ND 3.0](https://creativecommons.org/licenses/by-nc-nd/3.0/)*

You need two tools, yes, just two!:

- <img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/68e0fc81-9178-4291-96ac-8503d747331e" width="18" height="18"> **TrenchBroom** :
A modern level editor originally designed for  ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/7f2552fd-cfb4-4eb9-a6df-99f9b3551c06)
Quake, but it also supports  ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/90c0f277-55c9-45f0-af03-461b193ab42f)
Goldsrc engine games like  ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/c82b9b35-de85-4bdf-8d85-957300d59a19)
Counter-Strike 1.6.
  - [Download TrenchBroom](https://github.com/TrenchBroom/TrenchBroom/releases)
  
- ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/b347db29-a32e-43a9-a55e-7398bd4e99ab) **Map compile tools** :
  These tools convert the .map file created with TrenchBroom to a .bsp file, which Counter-Strike uses for maps.
  - [Download for Windows](https://github.com/twhl-community/VHLT-V34/releases)
  - [Download for Linux (requires GitHub account)](https://github.com/khanghugo/SDHLT/actions/runs/8559616842)

## Why TrenchBroom Instead of Valve Hammer Editor or J.A.C.K.?
![grids2](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/adff44ce-edac-4484-9379-a61bb89d58a9)

We know that traditional editors like ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/bb8f90f4-2733-4556-8367-501092a801e8) VHE and ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/24a58390-3f4b-43b0-9188-ec4ce9f8504c) J.A.C.K.
are the most recommended and widely used for mapping (in fact, 99.9% of KZ maps have been created with them). However, they have outdated interfaces and limit the brush creation to 2D views. In contrast, <img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/68e0fc81-9178-4291-96ac-8503d747331e" width="18" height="18"> TrenchBroom is designed primarily to use the 3D viewport for brush creation. That allows for an intuitive and natural approach to designing Kreedz maps since KZ is all about movement in 3D space. This makes it easier for new mappers to use. It's also worth mentioning that TrenchBroom supports 2D views.

> ##### Four features that TrenchBroom lacks.
> - The texturing tool isn’t easy to use; there are no buttons to ‘justify texture’ like adjusting the texture to the face.
> - It doesn't have a file browser to conveniently pick a sprite or model; you have to type paths manually in the cycler_sprite/env_sprite key value.
> - Skybox cannot be rendered.
> - Decals do not render with transparency.

---

## How to Start

**Extract TrenchBroom and Compile Tools into a Folder:**
   - From the VHLT zip, only extract the `tools` folder.
   - Example: `Mapping/tools`, `Mapping/TrenchBroom`.
   - For the Ubuntu version, it is automatically installed in `usr/share/TrenchBroom`.
          ![Screenshot from 2024-06-21 18-26-57](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/87a30114-a0fe-4b9e-b7aa-6558ca4484fb)

## Setup Editor

1. **Launch TrenchBroom:**
   - Click `New Map...` and then `Open preferences...`
          ![Screenshot from 2024-06-21 17-32-02](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/14db38f9-2dfc-4f45-8584-2bed76f3ecc0)

   - Select `Half-Life (experimental)`. Set the **Game Path** to where hl.exe is located. Click `Apply` and `OK`.
          ![Screenshot from 2024-06-21 17-36-47](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/b88f69e4-f825-4994-a51c-99a97c0f803f)



2. **Add the Compile Tools FGD to TrenchBroom Game Config:**
   - Copy `zhlt.fgd` from `Mapping/tools` and paste in `Mapping/Trenchbroom/Games/Halflife`
   - Create a new file and rename it as `combined.fgd`.
   - Open `combined.fgd` with a text editor and write this:
     ```plaintext
     @include "HalfLife.fgd"
     @include "zhlt.fgd"
     ```
   - Save the file.
       ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/90207e2a-dde5-43a2-841e-bac549d71c9d)

  
   - Open `GameConfig.cfg`, go to line 18, and replace “HalfLife.fgd” with “combined.fgd”.
       ![Screenshot from 2024-06-21 18-00-01](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/ec60d7c7-bc93-4bee-96b8-71ddeaf92a10)


3. **Finally Open TrenchBroom:**
   - Press `New map...`, select `Half-Life`, and press `OK`.
     ![Screenshot from 2024-06-21 18-10-41](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/65c3525f-21c7-4752-bad3-c9f4082581f5)

   - Add textures:
     - Go to the Entity tab, select the `wad` key, then press `+` below **Wad Files**, select  `zhlt.wad` from `Mapping/tools` and set the absolute path. Also add some wads from `cstrike` or `valve` folder.
       
       ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/60f76284-c426-4727-88a3-dc31e697a397)

       
   - Enable cstrike mod:
       
       ![Screenshot from 2024-06-21 18-13-20](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/8447d1cf-d8af-4990-b477-5aa110636494)


---

TrenchBroom is ready, but you still need to configure the compile tools. It's easy, let's see:

---

## Setup Compile Tools

1. Go to `Run > Compile Map…`, you will see a compile window with empty compilation profiles.
   ![Screenshot from 2024-06-21 18-18-33](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/bd94ea12-ca7d-4cde-83d9-76b26c652062)

3. Set a new profile. Press `+` to add a new profile. Add a custom name and `${GAME_DIR_PATH}/cstrike/maps` as the Working Directory.
   ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/d6945617-5518-4df5-8586-9c31514af8cd)


5. Add the following compilation tasks (1 Export task and 4 Run Tool tasks):

**Export Map**
   - File Path: `${WORK_DIR_PATH}/${MAP_BASE_NAME}.map`
   - This exports the map to the cstrike maps directory (working directory). If you want, you can add a second Export task for backup purposes with a different file path.

**Run Tool**
   - Tool Path: `Mapping/tools/hlcsg_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map" -nowadtextures`

**Run Tool**
   - Tool Path: `Mapping/tools/hlbsp_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map"`

**Run Tool**
   - Tool Path: `Mapping/tools/hlvis_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map" -full`

**Run Tool**
   - Tool Path: `Mapping/tools/hlrad_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map" -extra -bounce 4`
     
![Screenshot from 2024-06-21 18-52-06](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/609928b3-55bf-48ef-833a-faf6be3ad969)

---
## Now TrenchBroom is ready for KZ mapping.

 From now on you will only have to put your ideas into practice and let your imagination fly. Do what you want, no one will stop you. Do you want to make a map with only 257 LJ blocks? Do it. Do you want to create a Bhop map? Do it. Do you want to make a map with only edgebugs? Do it. Do you want to make a neon style death map? Don't do it, there are already plenty of ugly neon maps out there. GL & HF!

---

There is a template of a room with the start and end button (timer digits are not necessary as [kz plugins](https://kz-rush.ru/downloads.php) is used). Copy the next .map (in text format) to clipboard and paste them in TrenchBroom `Ctrl + V`. Add the halflife.wad from `valve` folder. Finally add the blocks for jumps!. Press ![NoTool](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/6d3bac21-6381-478c-bb7e-f34a11f0e692) and just click & drag the blocks in the 3D View, then you can modify the dimensions extruding the faces holding `SHIFT` and selecting the face to extrude.

![2024-06-2210-57-22-ezgif com-video-to-gif-converter](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/9c602be1-8a39-4539-8468-2e315f3ab57e)


![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/39002baf-2339-4d22-93f5-4a3e8a4f16ac)

```
// Game: Half-Life
// Format: Valve
// entity 0
{
"mapversion" "220"
"wad" "steam/steamapps/common/Half-Life/valve/halflife.wad"
"classname" "worldspawn"
"_tb_mod" "cstrike"
// brush 0
{
( -960 -64 16 ) ( -960 64 -16 ) ( -960 64 16 ) FIFTIES_WALL14V [ 0 -1 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 -1024 16 ) ( -960 -1024 -16 ) ( -960 -1024 16 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 -64 ) ( -960 -64 -64 ) ( 960 -64 -64 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 64 0 ) ( -960 -64 0 ) ( -960 64 0 ) C1A3FLOOR02 [ 1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 896 16 ) ( -960 896 -16 ) ( 960 896 -16 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 16 ) ( 960 -64 -16 ) ( 960 -64 16 ) FIFTIES_WALL14V [ 0 1 0 0 ] [ 0 0 -1 0 ] 0 1 1
}
// brush 1
{
( -1024 64 16 ) ( -1024 -64 16 ) ( -1024 -64 -16 ) FIFTIES_WALL14V [ 0 1 0 0 ] [ 0 0 -1 0 ] 0 1 1
( -1024 -1024 16 ) ( -2944 -1024 -16 ) ( -2944 -1024 16 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( -1024 64 0 ) ( -2944 -64 0 ) ( -1024 -64 0 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( -1024 64 640 ) ( -2944 -64 640 ) ( -2944 64 640 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( -1024 896 16 ) ( -2944 896 -16 ) ( -1024 896 -16 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( -960 64 16 ) ( -960 -64 -16 ) ( -960 -64 16 ) OUT_WALL7F [ -2.220446049250313e-16 1 0 64 ] [ 0 0 -1 0 ] 0 1 1
}
// brush 2
{
( -960 -64 16 ) ( -960 64 -16 ) ( -960 64 16 ) FIFTIES_WALL14V [ 0 -1 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 896 16 ) ( 960 896 -16 ) ( -960 896 -16 ) OUT_WALL7F [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 0 ) ( -960 -64 0 ) ( 960 -64 0 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 64 640 ) ( -960 -64 640 ) ( -960 64 640 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 960 16 ) ( -960 960 -16 ) ( 960 960 -16 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 16 ) ( 960 -64 -16 ) ( 960 -64 16 ) FIFTIES_WALL14V [ 0 1 0 0 ] [ 0 0 -1 0 ] 0 1 1
}
// brush 3
{
( -960 -2048 16 ) ( -960 -1920 -16 ) ( -960 -1920 16 ) FIFTIES_WALL14V [ 0 -1 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 -1088 16 ) ( 960 -1088 -16 ) ( -960 -1088 -16 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 -1920 0 ) ( -960 -2048 0 ) ( 960 -2048 0 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 -1920 640 ) ( -960 -2048 640 ) ( -960 -1920 640 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 -1024 16 ) ( -960 -1024 -16 ) ( 960 -1024 -16 ) OUT_WALL7F [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 -1920 16 ) ( 960 -2048 -16 ) ( 960 -2048 16 ) FIFTIES_WALL14V [ 0 1 0 0 ] [ 0 0 -1 0 ] 0 1 1
}
// brush 4
{
( -960 -64 720 ) ( -960 64 688 ) ( -960 64 720 ) FIFTIES_WALL14V [ 0 -1 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 -1024 720 ) ( -960 -1024 688 ) ( -960 -1024 720 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 640 ) ( -960 -64 640 ) ( 960 -64 640 ) LAB1_FLOOR4 [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 64 704 ) ( -960 -64 704 ) ( -960 64 704 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 896 720 ) ( -960 896 688 ) ( 960 896 688 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 720 ) ( 960 -64 688 ) ( 960 -64 720 ) FIFTIES_WALL14V [ 0 1 0 0 ] [ 0 0 -1 0 ] 0 1 1
}
// brush 5
{
( 960 64 16 ) ( 960 -64 16 ) ( 960 -64 -16 ) OUT_WALL7F [ -2.220446049250313e-16 -1 0 -64 ] [ 0 0 -1 0 ] 0 1 1
( 960 -1024 16 ) ( -960 -1024 -16 ) ( -960 -1024 16 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 0 ) ( -960 -64 0 ) ( 960 -64 0 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 64 640 ) ( -960 -64 640 ) ( -960 64 640 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 896 16 ) ( -960 896 -16 ) ( 960 896 -16 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 1024 64 16 ) ( 1024 -64 -16 ) ( 1024 -64 16 ) FIFTIES_WALL14V [ 0 1 0 0 ] [ 0 0 -1 0 ] 0 1 1
}
}
// entity 1
{
"classname" "info_player_start"
"spawnflags" "0"
"angles" "0 90 0"
"origin" "0 688 36"
}
// entity 2
{
"classname" "func_button"
"speed" "5"
"sounds" "0"
"wait" "3"
"delay" "0"
"spawnflags" "1"
"locked_sound" "0"
"unlocked_sound" "0"
"locked_sentence" "0"
"unlocked_sentence" "0"
"rendermode" "0"
"rendercolor" "0 0 0"
"renderfx" "0"
"angles" "0 0 0"
"zhlt_lightflags" "0"
"targetname" "counter_start_button"
"master" "power"
"target" "counter_start"
// brush 0
{
( -16 832 0 ) ( -16 833 0 ) ( -16 832 1 ) BLACK [ 0 -1 0 0 ] [ 0 0 -1 0 ] 0 1 1
( -32 864 0 ) ( -32 864 1 ) ( -31 864 0 ) BLACK [ -1 -2.220446049250313e-16 0 16 ] [ -4.930380657631324e-32 2.7755575615628914e-16 1 0 ] 0 1 1
( -16 864 32 ) ( -16 880 64 ) ( 112 880 64 ) +0BUTTON3 [ 1 0 0 -16 ] [ 0 -0.447213595499958 -0.894427190999916 2.7913208 ] 0 1 1
( -32 832 0 ) ( -31 832 0 ) ( -32 833 0 ) LAB1_FLOOR4 [ -1 0 0 32 ] [ 0 -1 0 0 ] 0 1 1
( 32 896 64 ) ( 32 897 64 ) ( 33 896 64 ) BLACK [ 0 -1 0 0 ] [ -1 0 -2.220446049250313e-16 16 ] 0 1 1
( 32 896 64 ) ( 33 896 64 ) ( 32 896 65 ) LAB1_FLOOR4 [ -1 0 0 32 ] [ 0 0 -1 0 ] 0 1 1
( 16 896 64 ) ( 16 896 65 ) ( 16 897 64 ) BLACK [ 0 -1 0 0 ] [ -2.7755575615628914e-16 0 1 0 ] 0 1 1
}
}
// entity 3
{
"classname" "func_button"
"speed" "5"
"sounds" "0"
"wait" "3"
"delay" "0"
"spawnflags" "1"
"locked_sound" "0"
"unlocked_sound" "0"
"locked_sentence" "0"
"unlocked_sentence" "0"
"rendermode" "0"
"rendercolor" "0 0 0"
"renderfx" "0"
"angles" "0 0 0"
"zhlt_lightflags" "0"
"targetname" "counter_stop_button"
"master" "stopsource"
"target" "counter_off"
// brush 0
{
( -16 -1024 64 ) ( -16 -1024 65 ) ( -16 -1025 64 ) BLACK [ 1.2246467991473532e-16 1 0 0 ] [ 2.7755575615628914e-16 -3.399077683617228e-32 1 0 ] 180 1 1
( -32 -1024 64 ) ( -33 -1024 64 ) ( -32 -1024 65 ) LAB1_FLOOR4 [ 1 -1.2246467991473532e-16 0 32 ] [ 0 0 -1 0 ] 180 1 1
( 32 -960 0 ) ( 31 -960 0 ) ( 32 -961 0 ) LAB1_FLOOR4 [ 1 -1.2246467991473532e-16 0 32 ] [ 1.2246467991473532e-16 1 0 32 ] 180 1 1
( -32 -1024 64 ) ( -32 -1025 64 ) ( -33 -1024 64 ) BLACK [ 1.2246467991473532e-16 1 0 0 ] [ 1 -1.2246467991473532e-16 -2.220446049250313e-16 16 ] 180 1 1
( 16 -992 32 ) ( 16 -1008 64 ) ( -112 -1008 64 ) +0BUTTON2 [ -1 1.2246467991473532e-16 0 -16 ] [ 5.476786982642027e-17 0.447213595499958 -0.894427190999916 28.034607 ] 180 1 1
( 32 -992 0 ) ( 32 -992 1 ) ( 31 -992 0 ) BLACK [ 1 9.957992501029599e-17 0 16 ] [ 1.531302974014096e-32 -2.7755575615628914e-16 1 0 ] 180 1 1
( 16 -960 0 ) ( 16 -961 0 ) ( 16 -960 1 ) BLACK [ 1.2246467991473532e-16 1 0 0 ] [ 0 0 -1 0 ] 180 1 1
}
}
// entity 4
{
"classname" "light"
"spawnflags" "0"
"_light" "255 255 128 200"
"style" "0"
"_fade" "1.0"
"_falloff" "0"
"origin" "8 760 152"
}
// entity 5
{
"classname" "light"
"spawnflags" "0"
"_light" "255 255 128 200"
"style" "0"
"_fade" "1.0"
"_falloff" "0"
"origin" "8 456 152"
}
// entity 6
{
"classname" "light"
"spawnflags" "0"
"_light" "255 255 128 200"
"style" "0"
"_fade" "1.0"
"_falloff" "0"
"origin" "8 104 152"
}
// entity 7
{
"classname" "light"
"spawnflags" "0"
"_light" "255 255 128 200"
"style" "0"
"_fade" "1.0"
"_falloff" "0"
"origin" "8 -232 152"
}
// entity 8
{
"classname" "light"
"spawnflags" "0"
"_light" "255 255 128 200"
"style" "0"
"_fade" "1.0"
"_falloff" "0"
"origin" "8 -616 152"
}
// entity 9
{
"classname" "light"
"spawnflags" "0"
"_light" "255 255 128 200"
"style" "0"
"_fade" "1.0"
"_falloff" "0"
"origin" "8 -920 152"
}
```

---

> Each community has its own rules for submitting maps, be sure you follow them if you want your map to be accepted.

<img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/0b27ca97-abf0-497e-b320-0ecd00a233ac" width="20" height="20"> [XJ Rules](https://xtreme-jumps.eu/upload-map)

<img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/b5dbf82d-7791-4f27-aca9-ddceaf978b8a" width="20" height="20"> [Cosy-Climbing Rules](https://cosy-climbing.net/map_suggest.php#rules)

<img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/422e5229-7852-4b62-af7f-c26439da8715" width="20" height="20"> [KZ-Rush Rules](https://kz-rush.ru/en/article/rules-for-maps-with-rush-tag)

![image](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/1600b235-52b6-479c-a468-d1d3197d2f0e/ddpcsvg-878bf78e-81e9-485c-8f9c-51d6ceac03b9.png/v1/fill/w_1600,h_900,q_80,strp/bhop_wallpaper__bhop_interloper_v1__by_nyu_one_ddpcsvg-fullview.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9OTAwIiwicGF0aCI6IlwvZlwvMTYwMGIyMzUtNTJiNi00NzljLWE0NjgtZDFkMzE5N2QyZjBlXC9kZHBjc3ZnLTg3OGJmNzhlLTgxZTktNDg1Yy04ZjljLTUxZDZjZWFjMDNiOS5wbmciLCJ3aWR0aCI6Ijw9MTYwMCJ9XV0sImF1ZCI6WyJ1cm46c2VydmljZTppbWFnZS5vcGVyYXRpb25zIl19.s16cMnii1FCKdxdLsmayGmYDpF9vFQSAM2jHLyxxLrA)

###### Image by [Nyu-One](https://www.deviantart.com/nyu-one) under [CC BY-NC-ND 3.0](https://creativecommons.org/licenses/by-nc-nd/3.0/)*

---

### Recommended Resources

- [The TrenchBroom Manual](https://trenchbroom.github.io/manual/latest/)
- [TrenchBroom Video Tutorials by dumptruck_ds](https://www.youtube.com/watch?v=gONePWocbqA&list=PLgDKRPte5Y0AZ_K_PZbWbgBAEt5xf74aE)
- [Bal's TrenchBroom Tips & Tricks](https://www.slipseer.com/index.php?threads/bals-quake-mapping-tips-tricks.100/)
- [TWHL: The largest website related to GoldSrc](https://twhl.info/wiki)
- [Xtreme-Jumps.eu Mapping Discord](https://discord.com/invite/AkggjC8PhF)
- [Advanced VHLT compilation parameters & tips](https://archive.svencoop.com.br/web/svencoop/20230220030651/https://sites.google.com/site/svenmanor/tutorials/advancedlight)
