include_directories(../src)
add_executable(wiiusemain main.c)
target_link_libraries(wiiusemain wiiuse)

if(INSTALL_EXAMPLES)
	install(TARGETS wiiuseexample
		RUNTIME DESTINATION bin COMPONENT main)
endif()