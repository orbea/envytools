project(ENVYTOOLS C)
cmake_minimum_required(VERSION 2.6)

add_library(nvhw chipset.c tile.c comp.c mpeg_crypt.c
	pgraph.c pgraph_xy.c fp.c sfu.c sfu_tab.c)

install(TARGETS nvhw
	RUNTIME DESTINATION bin
	LIBRARY DESTINATION lib${LIB_SUFFIX}
	ARCHIVE DESTINATION lib${LIB_SUFFIX})
