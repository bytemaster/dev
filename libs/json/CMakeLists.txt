SET( headers 
    value.hpp
    )
     
SET( sources
    value.cpp
   )

SET( libraries 
     ${Boost_SYSTEM_LIBRARY} 
     ${Boost_THREAD_LIBRARY} 
   )

include_directories( ../ )
INCLUDE_DIRECTORIES( ${Boost_INCLUDE_DIR} )
include_directories( /usr/include )

INCLUDE( SetupTargetMacros )

SETUP_LIBRARY( json  SOURCES   ${sources}
                       LIBRARIES ${libraries} 
                       AUTO_INSTALL_HEADERS 
                       LIBRARY_TYPE ${LIBRARY_BUILD_TYPE} )
