
file(
	GLOB
	COINUTILS_HEADER
	*.hpp
	*.h
)
file(
	GLOB
	COINUTILS_CPP
	*.cpp
)


ADD_LIBRARY(lib_CoinUtils ${COINUTILS_HEADER} ${COINUTILS_CPP})
INSTALL(TARGETS lib_CoinUtils DESTINATION lib EXPORT aliceVision-targets)
