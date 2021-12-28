# CMake-Error-when-running-png2ico

Hello World! I'm trying to compile the client-building from https://github.com/nextcloud/client-building

However, got stucked at CMake as shown in the last line in build-log: https://github.com/AkhmalFirdaus/CMake-Error-when-running-png2ico/blob/main/last-build-2021-12-28-09-18-22-Release.log.

Hence, I'm looking for the help from all github community to assist me in solving this issue.

1) Input:
```
In Git-Bash:  ../c/Nextcloud/client-building (master)
$ BUILD_INSTALLER=0 USE_CODE_SIGNING=0 UPLOAD_BUILD=0 ./task-build-log.bat
```

Output: (LN6676-LN6687)
```
..
CMake Error at cmake/modules/ECMAddAppIcon.cmake:113 (message):
  No ICONS argument given to ecm_add_app_icon
Call Stack (most recent call first):
  src/gui/CMakeLists.txt:362 (ecm_add_app_icon)


-- Configuring incomplete, errors occurred!
See also "C:/Nextcloud/client-building/desktop/build/CMakeFiles/CMakeOutput.log".
See also "C:/Nextcloud/client-building/desktop/build/CMakeFiles/CMakeError.log".
"*** Build FAILED: desktop Release Win64 (single-build-desktop.bat)"
"***** Build FAILED (build.bat)"
--- END: C:\Nextcloud\client-building\task-build-log.bat - 2021-12-28 09:22:38 ---
```

***

Other Error Log Location:
C:\Nextcloud\client-building\desktop\build\CMakeFiles

2) CMakeError.log: https://github.com/AkhmalFirdaus/CMake-Error-when-running-png2ico/blob/main/CMakeError.log

What is the meaning of deprecated? How to solve this issue?
````
...
Source file was:
__attribute__((__deprecated__)) int somefunc() { return 0; }
    int main() { return somefunc();}
````


3) CMakeOutput.log: https://github.com/AkhmalFirdaus/CMake-Error-when-running-png2ico/blob/main/CMakeOutput.log

Same as in CMakeError.log. What is the meaning of __declspec(deprecated)..? How to solve this issue?
````
...
Source file was:
__declspec(deprecated) int somefunc() { return 0; }
    int main() { return somefunc();}
````

Open for suggestions and help from all developers out there! 

Many Thanks!
