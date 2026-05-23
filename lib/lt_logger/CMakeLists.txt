
add_library(lt_logger INTERFACE)
target_include_directories(lt_logger INTERFACE ${CMAKE_CURRENT_LIST_DIR})
target_link_libraries(lt_logger INTERFACE pico_stdlib hardware_dma hardware_spi)

target_sources(lt_logger INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}/lt_logger.c 
    ${CMAKE_CURRENT_LIST_DIR}/lt_logger.h
    ${CMAKE_CURRENT_LIST_DIR}/lt_config.h
)


