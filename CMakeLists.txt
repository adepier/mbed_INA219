 
set(INA219_SOURCES INA219.cpp) 
add_library(mbed_INA219 STATIC ${INA219_SOURCES})
target_link_libraries( mbed_INA219 mbed-os)

set(INA219_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR} )
target_include_directories(mbed_INA219 PUBLIC ${INA219_HEADER_DIR})