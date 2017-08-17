set(SRCS
	src/AAFilter.cpp
	src/BPMDetect.cpp
	src/cpu_detect_x86.cpp
	src/FIFOSampleBuffer.cpp
	src/FIRFilter.cpp
	src/InterpolateCubic.cpp
	src/InterpolateLinear.cpp
	src/InterpolateShannon.cpp
	src/mmx_optimized.cpp
	src/PeakFinder.cpp
	src/RateTransposer.cpp
	src/SoundTouch.cpp
	src/sse_optimized.cpp
	src/TDStretch.cpp)

add_library(SoundTouch STATIC ${SRCS})
target_include_directories(SoundTouch PUBLIC include PRIVATE src)
