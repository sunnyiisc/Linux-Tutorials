Matlab Installation:
====================

Before installation steps:
--------------------------
Installing new Library:

Step-1:
    sudo yum install libnsl

Step-2:
    install matlab by runnning the "install" file in setup
    
Step-3:
    Launching:
        goto installed directory then ./bin/matlab

        
For more information: https://in.mathworks.com/matlabcentral/answers/399207-matlab-does-not-start-on-fedora-28?s_tid=answers_rc1-1_p1_MLT

Creating Shortcut after installation:
-------------------------------------
Step-1:
    Goto bin:
    cd /usr/local/bin
    
Step-2:
    creating link of the original file here:
    sudo ln -s <address of original file (eg:/MATLAB/R2018b/bin/matlab)> matlab
    //this will make youo call "matlab" in terminal from anywhere to open matab
    // example: sudo ln -s /run/media/sunny-iisc/Extras/0-LINUX/Softwares/MATLAB/R2018b/bin/matlab matlab

