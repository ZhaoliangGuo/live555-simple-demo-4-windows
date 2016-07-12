## 1. live555-simple-demo
Build the live555 in the VS2010(Debug/Release/Debug64/Release64).
 
- live555SDK : build the live555 lib  
- live555MediaServer : a simplest rtsp server demo   
- openRTSP : a simplest rtsp client demo 

## 2. Detailed Structure
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
## 3. Instructions.
###  - Build the live555SDK
After build the live555SDK, BasicUsageEnvironment.lib groupsock.lib liveMedia.lib UsageEnvironment.lib will be generated in the responding directory. For example, if you build in the Debug mode, that four lib mentioned above will be copied to `live555SDK\lib\Debug`, and if you build in the Release mode, these will be copied to `live555SDK\lib\Release`.

After build the live555SDK, all the headers needed will be copied to `live555SDK\include`.
### - Use the live555 lib.
Copy the `live555SDK\include` and `live555SDK\lib` to your VS2010 project, then configure the header path and the lib path, you can use the live555 lib.


