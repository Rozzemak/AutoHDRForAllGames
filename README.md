# AutoHDRForAllGames
Simple instruction on how to enable autohdr in every game.


1) Use this tool on every directx11+ and vulkan game to force autohdr: https://github.com/ledoge/autohdr_force -> and proceed to 2c) if the game uses vulkan
2) If the game is older and supports only directx9, use DXVK: https://github.com/doitsujin/dxvk (perfectly safe for all games, this is a part of what  steamdeck uses to run games on linux)
2a) You have to create dxvk.conf file with this content to enable HDR while you use dxvk: "dxgi.enableHDR = True" (without the " " symbols.) The file should contain only one row.
2c) Set a setting in Nvidia Control Panel -> Manage 3d settings -> scroll all the way down -> "Vulkan/OpenGL present method" => Prefer layered on DXGI swapchain" 
2d) This driver setting will reset itself every time you upgrade you nvidia driver
3) This will also allow you to use reshade cactus fix on older games to tweak hdr even more.
