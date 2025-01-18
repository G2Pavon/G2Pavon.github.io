
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
  - [Download for Windows](https://github.com/seedee/SDHLT/releases)
  - [Download for Linux (from Actions which requires GitHub account)](https://github.com/szGabu/SDHLT_Linux/actions/runs/12523659422)

## Why TrenchBroom Instead of Valve Hammer Editor or J.A.C.K.?
![grids2](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/adff44ce-edac-4484-9379-a61bb89d58a9)

We know that traditional editors like ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/bb8f90f4-2733-4556-8367-501092a801e8) VHE and ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/24a58390-3f4b-43b0-9188-ec4ce9f8504c) J.A.C.K.
are the most recommended and widely used for mapping (in fact, 99.9% of KZ maps have been created with them). However, they have outdated interfaces and limit the brush creation to 2D views. In contrast, <img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/68e0fc81-9178-4291-96ac-8503d747331e" width="18" height="18"> TrenchBroom is designed primarily to use the 3D viewport for brush creation. That allows for an intuitive and natural approach to designing Kreedz maps since KZ is all about movement in 3D space. This makes it easier for new mappers to use. It's also worth mentioning that TrenchBroom supports 2D views.

---

#### Here is a YouTube video showing the making of a kz map
  
  [![Trenchbroom showcase](http://img.youtube.com/vi/fnUfOF2Vjxw/0.jpg)](
  https://www.youtube.com/watch?v=fnUfOF2Vjxw)

---

## How to Start

**Extract TrenchBroom and Compile Tools into a Folder:**
   - From the VHLT zip, only extract the `tools` folder.
   - Example: `Mapping/tools`, `Mapping/TrenchBroom`.
   > LINUX USER: Since TrenchBroom 2024.2 only is release as Appimage, you will have to do an extra step in "Add the Compile Tools FGD to TrenchBroom Game Config:"

![Screenshot from 2025-01-18 09-18-17](https://github.com/user-attachments/assets/07098a8b-0d1f-41c8-b5fe-f58f5d95b2ca)

|tools|trenchbroom|
|------------|--------|
|       ![Screenshot from 2025-01-18 09-20-07](https://github.com/user-attachments/assets/01fff485-aa40-444b-abe2-92c0af53ec9c) |![image](https://github.com/user-attachments/assets/01609ce7-8057-402b-8dbf-123a07a9a717) |

## Setup Editor

1. **Launch TrenchBroom:**
   > LINUX user: set permission to "Executable as a program"

   - Click `New Map...` and then `Open preferences...`
![image](https://github.com/user-attachments/assets/ddb99612-1ecd-4eb4-b117-8824dfb22fff)


      ![image](https://github.com/user-attachments/assets/2287cdef-97dd-41a0-9b7b-72b1652328ca)


   - Select `Half-Life (experimental)`. Set the **Game Path** to half-life steamapps directory and also set map compiler tools  executables. Click `Apply` and `OK`.
          ![image](https://github.com/user-attachments/assets/c840b743-ff76-4654-a16f-7ff46aa771fe)





3. **Add the Compile Tools FGD to TrenchBroom Game Config:**

   > LINUX user: you have to do an extra step. Download [`app/resources/games`](https://github.com/TrenchBroom/TrenchBroom/tree/master/app/resources/games) folder from TB github repository and extract them in `~/.TrenchBroom/` aka `Home/.Trenchbroom/`. ![image](https://github.com/user-attachments/assets/626ab476-b78b-4252-8b47-56f8cc228f00) actually only need Halflife folder, but in case you ever want to mapping in other games...



   - Copy `sdhlt.fgd` from `Mapping/tools` and paste in `Mapping/Trenchbroom/Games/Halflife` (`Home/.Trenchbroom/games/Halflife` in linux)
   - Create a new text file in `games/Halflife` and rename it as `combined.fgd`.
   - Open `combined.fgd` with a text editor and write this:
     ```plaintext
     @include "HalfLife.fgd"
     @include "zhlt.fgd"
     ```
   - Save file.
       ![image](https://github.com/user-attachments/assets/7a9a7eaa-62af-4536-8932-f949ef72203b)



  
   - Open `GameConfig.cfg`, go to line 21, and replace `"definitions": [ "HalfLife.fgd" ]` with `"definitions": [ "combined.fgd" ]`.
       ![image](https://github.com/user-attachments/assets/9d07fe0e-a190-4d23-8d18-fa1a539db5e8)



5. **Finally Open TrenchBroom:**
   - Go to `Mapping/Trenchbroom/` and run it, then press `New map...`, select `Half-Life`, and press `OK`. ![image](https://github.com/user-attachments/assets/cde99950-129a-438f-9a7f-134720efb5e3)
  
     ![image](https://github.com/user-attachments/assets/1fb6c2ec-d213-479f-8489-99413252de65)

  - Enable cstrike mod:
      - Select `cstrike` and press `+`

      ![image](https://github.com/user-attachments/assets/545fb637-f422-44c7-b59e-57b98a5f96c0)


     
  - Add textures:
     - Go to the Entity tab in right panel (aka Entity Inspector), select worldspawn's `wad` key property, now below "Show default properties" a smart editor `Wad Files` is available, click `+` icon below **Wad Files** to add the wad files, select  `sdhlt.wad` from `Mapping/tools` and set absolute path type. Also add some wads from `cstrike` or `valve` folder.
       
      ![image](https://github.com/user-attachments/assets/d7886d9a-af01-418c-afa1-02a6570f622c)



---

TrenchBroom is ready, but you still need to configure the compile tools. It's easy, let's see:

---

## Setup Compile Tools

1. Go to `Run > Compile Map…`, you will see a compile window with empty compilation profiles.
       ![image](https://github.com/user-attachments/assets/73ee5cc9-e3e5-4584-a600-7f25cf3370b1)


3. Set a new profile. Click `+` in left panel to add a new profile. Add a custom name and `${GAME_DIR_PATH}/cstrike/maps` as the Working Directory.
   ![image](https://github.com/user-attachments/assets/705484e6-0ae9-45c0-a42a-49c8f490db2c)



5. Now add the following compilation tasks (1 Export Map and 4 Run Tool which are executed sequentially):

**Export Map**
   - File Path: `${WORK_DIR_PATH}/${MAP_BASE_NAME}.map`
   - This exports .map file to cstrike maps directory (aka working directory). If you want, you can add a second export task for backup purposes to a different path.

**Run Tool**
   - Tool Path: `${csg}`
   - Parameters: `${WORK_DIR_PATH}/${MAP_BASE_NAME}.map -nowadtextures`

**Run Tool**
   - Tool Path: `${bsp}`
   - Parameters: `${WORK_DIR_PATH}/${MAP_BASE_NAME}.map`

**Run Tool**
   - Tool Path: `${vis}`
   - Parameters: `${WORK_DIR_PATH}/${MAP_BASE_NAME}.map -full`

**Run Tool**
   - Tool Path: `${rad}` 
   - Parameters: `${WORK_DIR_PATH}/${MAP_BASE_NAME}.map -extra -threads ${CPU_COUNT}`
     
![image](https://github.com/user-attachments/assets/837b6cbe-cd73-4100-b06f-fa48767fb54a)


---

## Now TrenchBroom is ready for KZ mapping.

 From now on you will only have to put your ideas into practice and let your imagination fly. Do what you want, no one will stop you. Do you want to make a map with only 257 LJ blocks? Do it. Do you want to create a Bhop map? Do it. Do you want to make a map with only edgebugs? Do it. Do you want to make a neon style death map? Don't do it, there are already plenty of ugly neon maps out there. GL & HF!

---

There is a template of a room with the start and end button (timers are not necessary as [kz plugins](https://kz-rush.ru/downloads.php) is used, all you need is two func_button entities with *counter_start* and *counter_off* as target respectively. Anyway, if you want you can download timers from [here](https://github.com/G2Pavon/timercounter) ).


Copy next map (in text format) to clipboard and paste in TrenchBroom `Ctrl + V`. Add *halflife.wad* from `Half-Life/valve/`:


```

{
"mapversion" "220"
"wad" "/home/gaspar/.steam/steam/steamapps/common/Half-Life/valve/halflife.wad"
"classname" "worldspawn"
"_tb_mod" "cstrike"

{
( -960 -64 16 ) ( -960 64 -16 ) ( -960 64 16 ) FIFTIES_WALL14V [ 0 -1 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 -1024 16 ) ( -960 -1024 -16 ) ( -960 -1024 16 ) FIFTIES_WALL14V [ 1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 -64 ) ( -960 -64 -64 ) ( 960 -64 -64 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 64 0 ) ( -960 -64 0 ) ( -960 64 0 ) C1A3FLOOR02 [ 1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 896 16 ) ( -960 896 -16 ) ( 960 896 -16 ) FIFTIES_WALL14V [ -1 0 0 0 ] [ 0 0 -1 0 ] 0 1 1
( 960 64 16 ) ( 960 -64 -16 ) ( 960 -64 16 ) FIFTIES_WALL14V [ 0 1 0 0 ] [ 0 0 -1 0 ] 0 1 1
}

{
( -960 960 1280 ) ( -960 896 1280 ) ( -960 896 0 ) SKY [ -2.220446049250313e-16 0 1 0 ] [ 0 -1 0 0 ] 0 1 1
( -960 896 1280 ) ( 960 896 1280 ) ( 960 896 0 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 1 0 ] 0 1 1
( 960 896 0 ) ( 960 960 0 ) ( -960 960 0 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( -960 960 1280 ) ( 960 960 1280 ) ( 960 896 1280 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 960 0 ) ( 960 960 1280 ) ( -960 960 1280 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 -1 0 ] 0 1 1
( 960 896 1280 ) ( 960 960 1280 ) ( 960 960 0 ) SKY [ -2.220446049250313e-16 0 -1 0 ] [ 0 -1 0 0 ] 0 1 1
}

{
( -960 -1024 1280 ) ( -960 -1088 1280 ) ( -960 -1088 0 ) SKY [ -2.220446049250313e-16 0 1 0 ] [ 0 -1 0 0 ] 0 1 1
( -960 -1088 1280 ) ( 960 -1088 1280 ) ( 960 -1088 0 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 1 0 ] 0 1 1
( 960 -1088 0 ) ( 960 -1024 0 ) ( -960 -1024 0 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( -960 -1024 1280 ) ( 960 -1024 1280 ) ( 960 -1088 1280 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 -1024 0 ) ( 960 -1024 1280 ) ( -960 -1024 1280 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 -1 0 ] 0 1 1
( 960 -1088 1280 ) ( 960 -1024 1280 ) ( 960 -1024 0 ) SKY [ -2.220446049250313e-16 0 -1 0 ] [ 0 -1 0 0 ] 0 1 1
}

{
( -960 896 1344 ) ( -960 -1024 1344 ) ( -960 -1024 1280 ) SKY [ -2.220446049250313e-16 0 -1 0 ] [ 0 -1 0 0 ] 0 1 1
( -960 -1024 1344 ) ( 960 -1024 1344 ) ( 960 -1024 1280 ) SKY [ -4.930380657631324e-32 2.220446049250313e-16 -1 0 ] [ -1 -2.220446049250313e-16 0 0 ] 0 1 1
( 960 -1024 1280 ) ( 960 896 1280 ) ( -960 896 1280 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( -960 896 1344 ) ( 960 896 1344 ) ( 960 -1024 1344 ) SKY [ 1 0 -2.7755575615628914e-16 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 896 1280 ) ( 960 896 1344 ) ( -960 896 1344 ) SKY [ -4.930380657631324e-32 -2.220446049250313e-16 -1 0 ] [ 1 -2.220446049250313e-16 0 0 ] 0 1 1
( 960 -1024 1344 ) ( 960 896 1344 ) ( 960 896 1280 ) SKY [ -2.220446049250313e-16 0 -1 0 ] [ 0 -1 0 0 ] 0 1 1
}

{
( 960 896 1280 ) ( 960 -1024 1280 ) ( 960 -1024 0 ) SKY [ -2.220446049250313e-16 0 1 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 -1024 1280 ) ( 1024 -1024 1280 ) ( 1024 -1024 0 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 1 0 ] 0 1 1
( 1024 -1024 0 ) ( 1024 896 0 ) ( 960 896 0 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 960 896 1280 ) ( 1024 896 1280 ) ( 1024 -1024 1280 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( 1024 896 0 ) ( 1024 896 1280 ) ( 960 896 1280 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 -1 0 ] 0 1 1
( 1024 -1024 1280 ) ( 1024 896 1280 ) ( 1024 896 0 ) SKY [ -2.220446049250313e-16 0 -1 0 ] [ 0 -1 0 0 ] 0 1 1
}

{
( -1024 896 1280 ) ( -1024 -1024 1280 ) ( -1024 -1024 0 ) SKY [ -2.220446049250313e-16 0 1 0 ] [ 0 -1 0 0 ] 0 1 1
( -1024 -1024 1280 ) ( -960 -1024 1280 ) ( -960 -1024 0 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 1 0 ] 0 1 1
( -960 -1024 0 ) ( -960 896 0 ) ( -1024 896 0 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( -1024 896 1280 ) ( -960 896 1280 ) ( -960 -1024 1280 ) SKY [ -1 0 0 0 ] [ 0 -1 0 0 ] 0 1 1
( -960 896 0 ) ( -960 896 1280 ) ( -1024 896 1280 ) SKY [ -1 0 0 0 ] [ 0 -2.220446049250313e-16 -1 0 ] 0 1 1
( -960 -1024 1280 ) ( -960 896 1280 ) ( -960 896 0 ) SKY [ -2.220446049250313e-16 0 -1 0 ] [ 0 -1 0 0 ] 0 1 1
}
}

{
"classname" "func_button"
"speed" "5"
"wait" "3"
"delay" "0"
"spawnflags" "1"
"target" "counter_start"

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

{
"classname" "func_button"
"speed" "5"
"wait" "3"
"delay" "0"
"spawnflags" "1"
"target" "counter_off"

{
( -16 -1024 448 ) ( -16 -1024 449 ) ( -16 -1025 448 ) BLACK [ 1.2246467991473532e-16 1 0 0 ] [ 2.7755575615628914e-16 -3.399077683617228e-32 1 0 ] 180 1 1
( -32 -1024 448 ) ( -33 -1024 448 ) ( -32 -1024 449 ) LAB1_FLOOR4 [ 1 -1.2246467991473532e-16 0 32 ] [ 0 0 -1 0 ] 180 1 1
( 32 -960 384 ) ( 31 -960 384 ) ( 32 -961 384 ) LAB1_FLOOR4 [ 1 -1.2246467991473532e-16 0 32 ] [ 1.2246467991473532e-16 1 0 32 ] 180 1 1
( -32 -1024 448 ) ( -32 -1025 448 ) ( -33 -1024 448 ) BLACK [ 1.2246467991473532e-16 1 0 0 ] [ 1 -1.2246467991473532e-16 -2.220446049250313e-16 16 ] 180 1 1
( 16 -992 416 ) ( 16 -1008 448 ) ( -112 -1008 448 ) +0BUTTON2 [ -1 1.2246467991473532e-16 0 -16 ] [ 5.476786982642027e-17 0.447213595499958 -0.894427190999916 19.49469 ] 180 1 1
( 32 -992 384 ) ( 32 -992 385 ) ( 31 -992 384 ) BLACK [ 1 9.957992501029599e-17 0 16 ] [ 1.531302974014096e-32 -2.7755575615628914e-16 1 0 ] 180 1 1
( 16 -960 384 ) ( 16 -961 384 ) ( 16 -960 385 ) BLACK [ 1.2246467991473532e-16 1 0 0 ] [ 0 0 -1 0 ] 180 1 1
}
}

{
"classname" "info_player_start"
"spawnflags" "0"
"angles" "0 90 0"
"origin" "0 688 36"
}

{
"classname" "light_environment"
"pitch" "0"
"_light" "255 255 128 200"
"angles" "0 0 0"
"_fade" "1.0"
"_falloff" "0"
"origin" "8 792 120"
}

```

Finally add block for jumps!. How? click ![NoTool](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/6d3bac21-6381-478c-bb7e-f34a11f0e692) on Tool Bar and just click & drag the blocks in the 3D View, then select the brush and modify dimensions holding `SHIFT` and selecting the face to extrude. Also you can change grid size from Tool bar or with `+`/`-` keyboard buttons.

![image](https://github.com/user-attachments/assets/f653e344-0e94-4625-ae72-b6bfe18ae8da)


  ![2024-06-2210-57-22-ezgif com-video-to-gif-converter](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/9c602be1-8a39-4539-8468-2e315f3ab57e)


![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/912d678d-9a9c-4820-9865-48c4f5ee709d)

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
