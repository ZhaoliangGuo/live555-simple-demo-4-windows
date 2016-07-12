# live555-simple-demo
Build the live555 in the VS2010(Debug/Release/Debug64/Release64)

# Structure
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
