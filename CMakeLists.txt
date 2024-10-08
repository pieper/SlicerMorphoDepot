cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(MorphoDepot)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/MorphoDepot")
set(EXTENSION_CATEGORY "SlicerMorph")
set(EXTENSION_CONTRIBUTORS "Steve Pieper (Isomics, Inc.)")
set(EXTENSION_DESCRIPTION "Code to support collaborative segmentation projects using github.")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/MorphoDepot.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/MorphoDepot/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(MorphoDepot)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
