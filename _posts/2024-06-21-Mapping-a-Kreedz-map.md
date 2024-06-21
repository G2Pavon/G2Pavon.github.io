## How to Create a Kreedz Map

You only need two tools, yes only two things: 
- **TrenchBroom**: a modern level editor originally designed for Quake, but it also supports Goldsrc engine games like Counter-Strike 1.6.
  - [Download TrenchBroom](https://github.com/TrenchBroom/TrenchBroom/releases)
  
- **Map compile tools**: This tool converts the .map file created with TrenchBroom to a .bsp file, which Counter-Strike uses for maps.
  - [Download for Windows](https://github.com/twhl-community/VHLT-V34/releases)
  - [Download for Linux (requires GitHub account)](https://github.com/khanghugo/SDHLT/actions/runs/8559616842)

### Why TrenchBroom Instead of Valve Hammer Editor or J.A.C.K.?

While traditional editors like VHE and J.A.C.K. have their advantages (in fact, 99.9% of KZ maps have been created with them and they are excellent tools), TrenchBroom has a 3D-centered workflow and a modern interface. It allows for an intuitive and natural approach to designing Kreedz maps, as KZ is all about three-dimensional spatial movement, and that’s why I think it is more user-friendly for new mappers. It’s worth mentioning that TrenchBroom also supports 2D views, which I personally only use for precise vertex editing, especially when working with small grids.

#### The Only Four Drawbacks of TrenchBroom Compared to J.A.C.K:

- The texturing tool isn’t easy to use; there are no buttons to ‘justify texture’ like adjusting the texture to the face.
- It doesn't have a file browser to conveniently pick a sprite or model; you have to type paths manually in the cycler_sprite/env_sprite key value.
- Skyboxes cannot be previewed.
- Decals do not have transparency.

### How to Start

1. **Extract TrenchBroom and Compile Tools in the Same Folder:**
   - From the VHLT zip, only extract the `tools` folder.
   - Example: `Mapping/tools`, `Mapping/TrenchBroom`.
   - For the Ubuntu version, it is automatically installed in `usr/share/TrenchBroom`.
     ![Screenshot from 2024-06-21 18-26-57](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/87a30114-a0fe-4b9e-b7aa-6558ca4484fb)


2. **Launch TrenchBroom and Create a New Map:**
   ![Screenshot from 2024-06-21 18-06-46](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/4b0ffb0e-2b03-4f95-b425-e3fbce388e74)

   - Click `Open preferences...`
     
     ![Screenshot from 2024-06-21 17-32-02](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/14db38f9-2dfc-4f45-8584-2bed76f3ecc0)

   - Select `Half-Life (experimental)`. Set the Game Path to where hl.exe is located. Click `Apply` and `OK`.
     
     ![Screenshot from 2024-06-21 17-36-47](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/b88f69e4-f825-4994-a51c-99a97c0f803f)


4. **Add the Compile Tools FGD to TrenchBroom Configs:**
   - Go to the folder where TrenchBroom.exe is located, then go to `Games > Halflife`.

![Screenshot from 2024-06-21 17-46-00](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/a1e9ea57-7912-401c-8968-dd5f8331ec54)
![Screenshot from 2024-06-21 17-46-16](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/54da83ff-8993-4814-91ad-02b75a4d5cc1)



   - Copy `zhlt.fgd` from `Mapping/tools` and paste it here.

![Screenshot from 2024-06-21 17-49-27](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/99e2b7d1-880a-4ebb-8218-6831c07d6bef)

     
   - Create a new plain-text file with a text editor and rename it as `combined.fgd`.

![Screenshot from 2024-06-21 17-52-57](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/81570051-848e-453b-854a-ae607f8f655b)

     
   - Open `combined.fgd` with the text editor and add this:
     ```plaintext
     @include "HalfLife.fgd"
     @include "zhlt.fgd"
     ```

![Screenshot from 2024-06-21 17-54-35](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/23614cab-4116-4b9f-9dc6-a1f1b4382357)

     
   - Save the file.

4. **Configure GameConfig.cfg:**
   - Open `GameConfig.cfg`, go to line 18, and replace “HalfLife.fgd” with “combined.fgd”.

![Screenshot from 2024-06-21 17-58-16](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/df84df2b-bc0b-4d5b-9aa4-710e1a4b8eab)

![Screenshot from 2024-06-21 18-00-01](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/ec60d7c7-bc93-4bee-96b8-71ddeaf92a10)

---


5. **Open TrenchBroom:**
   - Press `New map`, select `Half-Life`, and press `OK`.

![Screenshot from 2024-06-21 18-10-41](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/65c3525f-21c7-4752-bad3-c9f4082581f5)

Extra: 

- Enable cstrike mod
  
This allows you to see Counter-Strike models as entities instead of Half-Life models.

![Screenshot from 2024-06-21 18-13-20](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/8447d1cf-d8af-4990-b477-5aa110636494)

- Add textures
  
  Go to Entity tab, select wad key, then press `+` below Wad files, select your .wad and then set absolute path
![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/7eaa0d06-f920-47c7-81bb-7e68eaf0cb7d)
![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/abf30f40-43b4-4fd9-97d9-5c4b531ea5af)





----


Now TrenchBroom is ready, but you still need to configure the compile tools. It's easy, let's see:

----

### Configure Compile Tools

1. Go to `Run > Compile Map…` You will see a compile window with empty compilation profiles.

![Screenshot from 2024-06-21 18-18-33](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/bd94ea12-ca7d-4cde-83d9-76b26c652062)

   
3. Set a new profile. Press `+ ` to add a new profile. Add a custom name and `${GAME_DIR_PATH}/cstrike/maps` as Working Directory

![image](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/d6945617-5518-4df5-8586-9c31514af8cd)



   
5. Add the following compilation tasks (1 Export task and 4 Run Tool tasks):

1. **Export Map**
   - File Path: `${WORK_DIR_PATH}/${MAP_BASE_NAME}.map`
   - This exports the map to the cstrike maps directory (working directory). If you want you can add a second Export task for backup purposes with a different file path

2. **Run Tool**
   - Tool Path: `Mapping/tools/hlcsg_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map" -nowadtextures`

3. **Run Tool**
   - Tool Path: `Mapping/tools/hlbsp_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map"`

4. **Run Tool**
   - Tool Path: `Mapping/tools/hlvis_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map" -full`

5. **Run Tool**
   - Tool Path: `Mapping/tools/hlrad_x64.exe`
   - Parameters: `"${WORK_DIR_PATH}/${MAP_BASE_NAME}.map" -extra -bounce 4`

![Screenshot from 2024-06-21 18-52-06](https://github.com/G2Pavon/G2Pavon.github.io/assets/14117486/609928b3-55bf-48ef-833a-faf6be3ad969)


Now TrenchBroom is finally ready for KZ mapping. From now on, all you need to do is put your ideas into practice and let your imagination soar. Create whatever you want—no one will stop you. Want to make a map with only 257 LJ blocks? Go for it. Want to create a bhop map? Do it. Want to design a map with edge bugs? Go ahead. Want to make a death map with a neon style? Maybe reconsider that one—there are already plenty of ugly neon maps out there. Happy mapping!

### Recommended Resources

- [The TrenchBroom Manual](https://kristianduske.com/trenchbroom/docs/latest/)
- [A complete YouTube guide on how to use TrenchBroom](https://www.youtube.com/playlist?list=PLNeRF-3NOXG8gg9WHP05mP2RRV8_5BdWl)
- [TWHL: The largest website with resources related to mapping in GoldSrc](https://twhl.info/)
- [Kreedz.com Mapping Discord](https://discord.gg/kreedz)
