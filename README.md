# HorusEyesRat
Remote Acess Tool Written in VB.NET



Features : 

* Multi-Threaded
* Packets Serialization
* Multi Ports Listener
* Automation Tasks when client is connected
* Save Settings for automation tasks
* Blur ScreenLocker
* Monitor Rotation (0 , 90 , 180 , 270 degrees)
* Hide & Show Taskbar
* Hide & Show Desktop Icons
* Hide & Show Cursor
* Swap & Normal State Mouse Buttons
* Lock & Unlock Keyboard
* Empty Bin
* Native Injection : You can inject an unmanaged DLL (C++ ,  C , D...)
* 32 & 64 bit stubs : pay attention when you want to inject Dll (ex : 32bit = dll 32 bit and 64bit = dll 64 bit for native)
* Mass Tasks: Passwords Recovery , History Recovery , Wifi Passwords Recovery
* Tasks Manager : Kill , Resume , Pause
* Passwords Recovery (+35 web browsers based on chromium)
* History Recovery (+35 web browsers based on chromium)
* Wifi Passwords Recovery
* Power : Log out , Reboot , Shutdown , Hibernate , Suspend
* BSOD
* Increase Volume
* Decrease Volume
* Mute | Unmute Volume
* Save all passwords | history recovered

Sources :

* Passwords Recovery : Modded Library Based on : https://github.com/0xfd3/Chrome-Password-Recovery
* Wifi Passwords Recovery : Modded Library Based on : https://github.com/r3nhat/SharpWifiGrabber
* Loading Unmanaged DLLs in Managed EXE : Class comes from : https://github.com/schellingb/DLLFromMemory-net with manual mapping for those dlls.
* Code I used to test the loading of dll in memory (in C++ but also worked in D Lang) : 

```
BOOL APIENTRY DllMain( HMODULE hModule,
                       DWORD  ul_reason_for_call,
                       LPVOID lpReserved
                     )
{
    switch (ul_reason_for_call)
    {
    case DLL_PROCESS_ATTACH:
        MessageBoxA(NULL, "Hello World!", "Dll says:", MB_OK);
    case DLL_THREAD_ATTACH:
    case DLL_THREAD_DETACH:
    case DLL_PROCESS_DETACH:
        break;
    }
    return TRUE;
}
```


Preview :

![Image description](https://i.postimg.cc/T2ZwvdVH/Capture-d-cran-15.png)
![Image description](https://i.postimg.cc/5NLtxhp9/Capture-d-cran-16.png)
![Image description](https://i.postimg.cc/SKTSTkQd/Capture-d-cran-17.png)
![Image description](https://i.postimg.cc/0yvyrVHY/Capture-d-cran-18.png)
![Image description](https://i.postimg.cc/LXJHGwnp/Capture-d-cran-19.png)
![Image description](https://i.postimg.cc/tgCRNYb7/Capture-d-cran-20.png)
![Image description](https://i.postimg.cc/JzQ4Xj99/Capture-d-cran-21.png)
