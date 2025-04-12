cmake_minimum_required(VERSION 3.18)

project(cpc C)

add_compile_options(-Wall -m64)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
# Add executable
add_executable(cpc cpc.c)

install(TARGETS cpc
        RUNTIME DESTINATION ${CMAKE_SOURCE_DIR})




# Enable device code linking
set_target_properties(cpc PROPERTIES
    OUTPUT_NAME "cpc.out"
)


# Set include directories
target_include_directories(cpc PRIVATE
   
)

# Set link directories
target_link_directories(cpc PRIVATE
    
)

# Link libraries
target_link_libraries(cpc PRIVATE

)
    