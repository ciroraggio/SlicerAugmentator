cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(SlicerAugmentator)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/SlicerAugmentator")
set(EXTENSION_CATEGORY "Utils")
set(EXTENSION_CONTRIBUTORS "Ciro Benito Raggio (KIT)")
set(EXTENSION_DESCRIPTION ".")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/SlicerAugmentator.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/SlicerAugmentator/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
