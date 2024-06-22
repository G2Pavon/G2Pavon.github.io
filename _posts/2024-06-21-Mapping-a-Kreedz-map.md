## How to Create a Kreedz Map

![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/97b7d9fa-fa0d-45cb-a839-9abb2c4efe11)


You only need two tools, yes, only two things:

- <img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/68e0fc81-9178-4291-96ac-8503d747331e" width="18" height="18"> **TrenchBroom**
: A modern level editor originally designed for  ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/7f2552fd-cfb4-4eb9-a6df-99f9b3551c06)
Quake, but it also supports  ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/90c0f277-55c9-45f0-af03-461b193ab42f)
Goldsrc engine games like  ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/c82b9b35-de85-4bdf-8d85-957300d59a19)
Counter-Strike 1.6.
  - [Download TrenchBroom](https://github.com/TrenchBroom/TrenchBroom/releases)
  
- ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/b347db29-a32e-43a9-a55e-7398bd4e99ab) **Map compile tools** 
: These tools convert the .map file created with TrenchBroom to a .bsp file, which Counter-Strike uses for maps.
  - [Download for Windows](https://github.com/twhl-community/VHLT-V34/releases)
  - [Download for Linux (requires GitHub account)](https://github.com/khanghugo/SDHLT/actions/runs/8559616842)

### Why TrenchBroom Instead of Valve Hammer Editor or J.A.C.K.?

We know that traditional editors like ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/bb8f90f4-2733-4556-8367-501092a801e8) VHE and ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/24a58390-3f4b-43b0-9188-ec4ce9f8504c) J.A.C.K.
are the most recommended and widely used for mapping (in fact, 99.9% of KZ maps have been created with them). However, they have outdated interfaces and limit the brush creation to 2D views. In contrast, <img src="https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/68e0fc81-9178-4291-96ac-8503d747331e" width="18" height="18"> TrenchBroom is designed primarily to use the 3D viewport for brush creation. That allows for an intuitive and natural approach to designing Kreedz maps since KZ is all about movement in 3D space. This makes it easier for new mappers to use. It's also worth mentioning that TrenchBroom supports 2D views.

#### The Only Four Drawbacks of TrenchBroom Compared to J.A.C.K:

- The texturing tool isn’t easy to use; there are no buttons to ‘justify texture’ like adjusting the texture to the face.
- It doesn't have a file browser to conveniently pick a sprite or model; you have to type paths manually in the cycler_sprite/env_sprite key value.
- Skyboxes cannot be previewed.
- Decals do not have transparency.

### How to Start

1. **Extract TrenchBroom and Compile Tools into a Folder:**
   - From the VHLT zip, only extract the `tools` folder.
   - Example: `Mapping/tools`, `Mapping/TrenchBroom`.
   - For the Ubuntu version, it is automatically installed in `usr/share/TrenchBroom`.
          ![Screenshot from 2024-06-21 18-26-57](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/87a30114-a0fe-4b9e-b7aa-6558ca4484fb)


2. **Launch TrenchBroom:**
   - Click `New Map...` and then `Open preferences...`
          ![Screenshot from 2024-06-21 17-32-02](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/14db38f9-2dfc-4f45-8584-2bed76f3ecc0)

   - Select `Half-Life (experimental)`. Set the **Game Path** to where hl.exe is located. Click `Apply` and `OK`.
          ![Screenshot from 2024-06-21 17-36-47](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/b88f69e4-f825-4994-a51c-99a97c0f803f)



4. **Add the Compile Tools FGD to TrenchBroom Game Config:**
   - Copy `zhlt.fgd` from `Mapping/tools` and paste in `Mapping/Trenchbroom/Games/Halflife`
   - Create a new file and rename it as `combined.fgd`.
   - Open `combined.fgd` with a text editor and write this:
     ```plaintext
     @include "HalfLife.fgd"
     @include "zhlt.fgd"
     ```
   - Save the file.
       ![Screenshot from 2024-06-21 17-52-57](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/81570051-848e-453b-854a-ae607f8f655b)
  
   - Open `GameConfig.cfg`, go to line 18, and replace “HalfLife.fgd” with “combined.fgd”.
       ![Screenshot from 2024-06-21 18-00-01](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/ec60d7c7-bc93-4bee-96b8-71ddeaf92a10)


5. **Finally Open TrenchBroom:**
   - Press `New map...`, select `Half-Life`, and press `OK`.
     ![Screenshot from 2024-06-21 18-10-41](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/65c3525f-21c7-4752-bad3-c9f4082581f5)

   - Add textures:
     - Go to the Entity tab, select the `wad` key, then press `+` below **Wad Files**, select  `zhlt.wad` from `Mapping/tools` and set the absolute path. Also add some wads from `cstrike` or `valve` folder.
       
       ![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/60f76284-c426-4727-88a3-dc31e697a397)

       
   - Enable cstrike mod:
     - This allows you to see Counter-Strike models as entities instead of Half-Life models.
       
       
       ![Screenshot from 2024-06-21 18-13-20](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/8447d1cf-d8af-4990-b477-5aa110636494)


---

TrenchBroom is ready, but you still need to configure the compile tools. It's easy, let's see:

---

### Configure Compile Tools

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


Now TrenchBroom is finally ready for KZ mapping. From now on, all you need to do is put your ideas into practice and let your imagination soar. Create whatever you want—no one will stop you. Want to make a map with only 257 LJ blocks? Go for it. Want to create a bhop map? Do it. Want to design a map with edge bugs? Go ahead. Want to make a death map with a neon style? Maybe reconsider that one—there are already plenty of ugly neon maps out there. Happy mapping!

### Recommended Resources

- [The TrenchBroom Manual](https://trenchbroom.github.io/manual/latest/)
- [TrenchBroom Video Tutorials by dumptruck_ds](https://www.youtube.com/watch?v=gONePWocbqA&list=PLgDKRPte5Y0AZ_K_PZbWbgBAEt5xf74aE)
- [TWHL: The largest website related to GoldSrc](https://twhl.info/wiki)
- [Xtreme-Jumps.eu Mapping Discord](https://discord.com/invite/AkggjC8PhF)
