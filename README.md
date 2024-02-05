# Setting up Dear ImGUI in CLion 

I have just started using CLion and I realized getting IMGUI setup for it was painful and there was not much documentation online so I thought it would be a good idea to do it once and push it to git so hopefully people with the same struggle can find this. 

Follow the Step by Step description or simply pull down my repository if you don't care which version you are getting.

## Step by Step:

1. Create a new CLion Project in my case its named DearIMGUI

2. In your terminal navigate to the folder of your project 

   ```
   cd CLionProjects/DearIMGUI
   ```

   

3. Clone the git repository for Dear IMGUI into a folder called imgui

   ```
   git submodule add https://github.com/ocornut/imgui imgui
   ```

   

4. Clone the git repository for GLFW into a folder called glfw

   ```
   git submodule add https://github.com/glfw/glfw.git glfw
   ```

   

5. Make sure you have vulkan installed and set the environment variables as follows 

   Download vulkan here -> https://vulkan.lunarg.com/sdk/home
   Run the installer and set up the following system variables in your Environment settings

   ```
   Vulkan_INCLUDE_DIR C:\VulkanSDK\1.3.275\Include
   Vulkan_LIBRARY C:\VulkanSDK\1.3.275\Lib
   ```

6. Write the CMakeLists.txt (use this repository as an example)

7. Run Dear IMGUI's sample for vulkan (see main.cpp of this repository)

8. Done
