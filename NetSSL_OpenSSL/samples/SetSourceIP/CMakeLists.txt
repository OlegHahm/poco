set(SAMPLE_NAME "SetSourceIP")

# uncomment following line, might solve compiling issues
#set(CMAKE_CXX_STANDARD 11)

set(LOCAL_SRCS "")
aux_source_directory(src LOCAL_SRCS)

add_executable( ${SAMPLE_NAME} ${LOCAL_SRCS} )
target_link_libraries( ${SAMPLE_NAME} PocoNetSSL PocoCrypto PocoUtil PocoNet PocoXML PocoFoundation )
