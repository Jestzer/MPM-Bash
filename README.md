# MPM, in Bash
A bash script that interacts with MATLAB Package Manager (MPM), which is a command-line-only installer for MathWorks.
Notes:
- This bash script is in no way affiliated with MathWorks.
- Now supports R2025b!
- You need an internet connection to use this. There is currently no option to specify "offline installation files".
- If you don't want to install all products, you need to use the same syntax as MPM to specify the products you want. This means different products should be separated with spaces and single products with spaces in their name should be replaced with underscores (ex: MATLAB Simulink MATLAB_Parallel_Server).
- When specifying products, you can use the shortcut "parallel_products" to select MATLAB, MATLAB Parallel Server, and Parallel Computing Toolbox. This will work for R2019a+.
- Specifying to install all products will not install any support packages.
- Use the argument "-version" to specify the script's version number.

To-do:
- Error out if mpm is not found and wget fails/isn't found
- Allow ~ to be used in file paths
