add_subdirectory(hyperiond)
add_subdirectory(hyperion-remote)

# The following clients depend on the protobuf library
if (ENABLE_AMLOGIC)
	add_subdirectory(hyperion-aml)
endif()

if(ENABLE_V4L2)
	add_subdirectory(hyperion-v4l2)
endif()

if(ENABLE_X11)
	add_subdirectory(hyperion-x11)
endif()

if(ENABLE_DISPMANX)
	add_subdirectory(hyperion-dispmanx)
endif()

if(ENABLE_FB)
	add_subdirectory(hyperion-framebuffer)
endif()

if(ENABLE_OSX)
	add_subdirectory(hyperion-osx)
endif()

