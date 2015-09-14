project(testfilter_tilde)
 
add_definitions(-DMSW)
 
set(SRC testfilter~.c)
 
include_directories("U:\pd\pd-win\pd\src")
link_directories("U:\pd\pd-win\pd\bin")
 
add_library(testfilter~ SHARED ${SRC} testfilter~.def)
 
target_link_libraries (testfilter~ pd)