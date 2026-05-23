add_library(
	fatfs
	${CMAKE_CURRENT_LIST_DIR}/source/ff.c
	${CMAKE_CURRENT_LIST_DIR}/source/ffsystem.c
	${CMAKE_CURRENT_LIST_DIR}/source/ffunicode.c
)

target_compile_options(fatfs PRIVATE --include=ffconfig.h)
target_include_directories(fatfs PUBLIC fatfs/source .)
