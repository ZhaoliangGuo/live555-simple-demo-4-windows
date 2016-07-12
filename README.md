## live555-simple-demo
Build the live555 in the VS2010(Debug/Release/Debug64/Release64).

After build the project, you can copy the 'include' and the 'lib' dir in the live555SDK to your project, and then after confiure the header path and the lib path, you can use the live555 lib.

## Structure
├─live555MediaServer  
|  
├─live555SDK  
│  ├─BasicUsageEnvironment  
│  │  └─include  
│  ├─groupsock  
│  │  └─include  
│  ├─include                  -- When build the live555SDK, all the header files needer will be copy to this dir.  
│  ├─lib                      -- When build the live555SDK, the responding .lib will be copy to this dir.   
│  │  ├─Debug                 -- Store the .lib when build in Debug mode.  
│  │  ├─Debug64               -- Store the .lib when bulid in Debug64 mode.  
│  │  ├─Release               -- Store the .lib when build in Release mode.  
│  │  └─Release64             -- Store the .lib when bulid in Release64 mode.  
│  ├─liveMedia  
│  │  └─include  
│  ├─mediaServer  
│  ├─proxyServer  
│  ├─testProgs  
│  └─UsageEnvironment  
│      └─include  
|  
└─openRTSP  
