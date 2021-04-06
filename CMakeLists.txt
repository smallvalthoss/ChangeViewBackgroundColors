cmake_minimum_required(VERSION 3.13.4)

project(ChangeBackGroundColour)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/ChangeBackGroundColour")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Walder (KnowThyselfProject)")
set(EXTENSION_DESCRIPTION "Simple Extension to pick the background colour in VR")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/ChangeBackGroundColour.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/ChangeBackGroundColour/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(ChangeBackGroundColourVR)
add_subdirectory(ChangeViewColors)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
