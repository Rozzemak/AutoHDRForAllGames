# AutoHDRForAllGames
Simple instruction on how to enable autohdr in every game.

 1. Use this tool on every directx11+ and vulkan game to force autohdr: https://github.com/ledoge/autohdr_force -> download it from the releases section, copy it to game folder and use it. That's all.  AND -> Proceed to 4) if the game uses vulkan.
 2.  If the game is older and supports only directx9, use DXVK: https://github.com/doitsujin/dxvk (perfectly safe for all games, this is a part of what  steamdeck uses to run games on linux)
 3. You have to create dxvk.conf file with this content to enable HDR while you use dxvk: "dxgi.enableHDR = True" (without the " " symbols.) The file should contain only one row. Its in this github repo, you can just use it.
 4. How to use dxvk ? Just download it from the releases tab, and put the dll files in your game folder. Same goes for config files.
 5. Set a setting in Nvidia Control Panel -> Manage 3d settings -> scroll all the way down -> "Vulkan/OpenGL present method" => Prefer layered on DXGI swapchain" 
 6. This driver setting will reset itself every time you upgrade you nvidia driver
 7. This will also allow you to use reshade cactus fix on older games to tweak hdr even more.

This repo was created as a way to contact one particular youtuber, 
because every time I post this guide into comment section, 
I get a shadow ban on comments by youtube allmighty algorythm. 
I cannot even mention the words: search, github in one sentence...
