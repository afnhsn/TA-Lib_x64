# TA-Lib x64 Download
TA-Lib x64; 64-bit ta-lib; Download;


Already compiled TA-Lib for 64 bit, you can just download and use it. 



I couldn’t find 64 bit “TA-Lib” library. I wanted to use it in 64 bit Python.  But I was getting the error below:
 ```
Creating library build\temp.win-amd64-3.5\Release\talib\common.cp35-win_amd64.lib and object build\temp.win-amd64-3.5\Release\talib\common.cp35-win_amd64.exp
common.obj : error LNK2001: unresolved external symbol TA_SetUnstablePeriod
common.obj : error LNK2001: unresolved external symbol TA_Shutdown
common.obj : error LNK2001: unresolved external symbol TA_Initialize
common.obj : error LNK2001: unresolved external symbol TA_GetUnstablePeriod
common.obj : error LNK2001: unresolved external symbol TA_GetVersionString
build\lib.win-amd64-3.5\talib\common.cp35-win_amd64.pyd : fatal error LNK1120: 5 unresolved externals
error: command 'C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC\BIN\x86_amd64\link.exe' failed with exit status 1120
 ```
 
 I found solution, but I had to install Visual Studio for it.
 
 Failed to install ta-lib
 https://github.com/mrjbq7/ta-lib/issues/127

![capture](https://user-images.githubusercontent.com/29254495/31372882-76034d84-ada0-11e7-96a4-ab3e49ca5cf5.PNG)
 
 I attached already Re Build TA-Lib Library for 64 bit
 
 Here are my instructions to build the 64-bit ta-lib.

Install TA-Lib C Library on Windows 10

    1. Download and Unzip ta-lib-0.4.0-msvc.zip
    2. Move the Unzipped Folder ta-lib to C:\
    3. Download and Install Visual Studio Community 2015
        Remember to Select [Visual C++] Feature
    4. Build TA-Lib Library
        From Windows Start Menu, Start [VS2015 x64 Native Tools Command Prompt]
        Move to C:\ta-lib\c\make\cdr\win32\msvc
        Build the Library nmake
    5. Then pip3 install ta-lib
    
 
 http://www.ta-lib.org/hdr_dw.html
 
  ![capture 2](https://user-images.githubusercontent.com/29254495/31372886-7a54336c-ada0-11e7-9c2b-16e04c0643f9.PNG)
 
 
