# qt-widgets-template

To use:

1. Find Qt installation path, and use Qt location as `CMAKE_PREFIX_PATH`
2. If using Visual Studio 2015 (some later versions change this) be sure
   you have 'developer prompt' setup "vcvarsall.bat"
  -   @echo ---- Launching QtCreator after setting 2015 MSVC 64-bit + WinSDK 10.0.10240.0 (as 10.0.26624)
  -   call "C:\Program Files (x86)\Microsoft Visual Studio 14.0\VC\vcvarsall.bat" amd64 10.0.10240.0
  -   echo --- trying to start QtCreator ---
  -   start "QtCreator" /B "C:\Qt\Qt5.9.1\Tools\QtCreator\bin\qtcreator.exe"
3. I suggest using NMake (normal makefiles with MSVC tools)
4. `mkdir build`
5. `cd build`
6. `cmake .. -DCMAKE_PREFIX_PATH=C:\Qt\Qt5.9.1\5.9.1\msvc2015_64 -G"NMake Makefiles" ` 
7. `make`

