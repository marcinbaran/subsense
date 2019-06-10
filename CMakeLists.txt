cmake_minimum_required(VERSION 2.8)
project( SuBSENSE )
find_package( OpenCV REQUIRED )
set(OpenCV_FOUND 1)
add_executable( SuBSENSE bgfg_segm.cpp
BackgroundSubtractorLBSP.cpp BackgroundSubtractorSuBSENSE.cpp LBSP.cpp)
target_link_libraries( SuBSENSE ${OpenCV_LIBS} )