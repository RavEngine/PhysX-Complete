# PhysX-Complete

The latest version of NVIDIA PhysX, with modifications to make it compile with CMake on more platforms.
Developed for use in [RavEngine](https://github.com/RavEngine/RavEngine). 

## How to use:
```cmake
add_subdirectory(physx-complete)

target_include_directories(your-app
	PUBLIC 
	"physx-complete/physx/physx/include/" 
	"physx-complete/physx/pxshared/include/" 
	"physx-complete/physx/physx/snippets/"
)

target_link_libraries(your-app PRIVATE 
	"PhysXExtensions"
	"PhysX"
	"PhysXPvdSDK"
	"PhysXVehicle"
	"PhysXCharacterKinematic"
	"PhysXCooking"
	"PhysXCommon"
	"PhysXFoundation"
	"PhysXTask"
	"FastXml"
	"LowLevel"
	"LowLevelAABB"
	"LowLevelDynamics"
	"SceneQuery"
	"SimulationController"
)
```

**Supported Platforms:**
- macOS (Intel and Apple Silicon)
- Windows Win32
- Windows UWP
- Linux
- iOS 
- AppleTV 
- WebAssembly / Emscripten


### Current Version
- PhysX 5.1.2 as of Dec 12, 2022 (No Blast yet)

### Contributing
Contributions are welcome. Please submit Issues if you find problems, and Pull Requests to address issues. If the problem is
within PhysX itself, submit your issues and pull requests there. 
