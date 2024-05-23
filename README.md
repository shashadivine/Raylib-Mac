# Raylib-Mac
A Raylib template for MacOS VSCode users.

Credits to people in this Reddit thread:
  https://www.reddit.com/r/raylib/comments/sh586x/hi_im_trying_to_get_raylib_to_work_on_mac_ive/
This Mac Raylib template is a combination of their tutorials, advice, and my experience with Raylib on MacOS VSCode.

STEPS
1. Create a folder/directory for your project (e.g. GameDev).
2. Install raylib on your machine.
3. Download the raylib-template branch and add it into your project directory (from Step 1)
- You may delete the README.md files in the bin, assets, and src folders. Here are some of their functionalities.
  - assets: You **may** place your asset files here (e.g. images, txt files, audio, etc.)
  - src: Your code files go in here (e.g. main.cpp)
  - bin: Your compiled binaries are stored here
  - lib: Contains essential raylib library contents
  - Makefile: CFILES = src/main.cpp | change 'main' to whatever file name you may have, or add onto it if you have more than 1 file for your project (e.g. main.cpp player.cpp).
4. There is a sample **main.cpp** file in src. Run it by choosing 'Run C/C++ File'. This option will show up if your file is present in Makefile.
5. An error message "The preLaunchTask 'Build.OSX' terminated with exit code 2." Choose 'Debug Anyway' and then select "Open 'launch.json'"
6. Copy paste the contents of the vscode-folder-content to their respective files. Usually 'settings.json' and 'c_cpp_properties.json' are not present, so make sure to add them in the .vscode folder as well.

After following these steps, you should now be able to run your code properly. Remember to include your relevant files in Makefile and use 'Run C/C++ File' to run your main code.

--- ALTERNATIVE SET-UP (after following steps) ---
(Usually helpful for groupworks, wherein not everyone has the same set up [Windows users])
- If all the files are in one place (e.g. not segregated into assets, src, etc.), you may remove 'src/' in Makefile.
- so it would look like 'Makefile: CFILES = main.cpp'

