## 1. live555-simple-demo
Build the live555 in VS2010(Debug/Release/Debug64/Release64).
 
- live555SDK : build the live555 lib  
- live555MediaServer : a simplest RTSP server applications demo   
- openRTSP : a simplest RTSP client demo 


> This code forms a set of C++ libraries for multimedia streaming, using open standard protocols (RTP/RTCP, RTSP, SIP).
These libraries can be used to build streaming applications. The libraries can also be used to stream, receive, and process MPEG, H.265, H.264, H.263+, DV or JPEG video, and several audio codecs. 
They can easily be extended to support additional (audio and/or video) codecs, and can also be used to build basic RTSP or SIP clients and servers, and have been used to add streaming support to existing media player applications, such as "VLC" and "MPlayer". 
http://www.live555.com/liveMedia/


## 2. Detailed Structure
├─live555MediaServer   
|  
├─live555SDK  
│  ├─BasicUsageEnvironment  
│  │  └─include  
│  ├─groupsock  
│  │  └─include  
│  ├─include                  -- When build the live555SDK, all the header files needer will be copy to this directory.  
│  ├─lib                      -- When build the live555SDK, the responding .lib will be copy to this directory.   
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
After build the live555SDK, `BasicUsageEnvironment.lib, groupsock.lib, liveMedia.lib, UsageEnvironment.lib` will be generated in the responding directory. e.g. If you build in the Debug mode, that four libs mentioned above will be copied to `live555SDK\lib\Debug`, and if you build in the Release mode, these will be copied to `live555SDK\lib\Release`.

After build the live555SDK, all the headers needed will be copied to `live555SDK\include`.
### - Use the live555 lib.
Copy the `live555SDK\include` and `live555SDK\lib` to your VS2010 project, then configure the header path and the lib path, you can use the live555 lib.


