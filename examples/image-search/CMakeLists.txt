set(CXX_STANDARD_REQUIRED ON)

add_executable(image-search-build
	usearch/index.hpp
	build.cpp
)

target_link_libraries(image-search-build PRIVATE clip ggml)

target_compile_features(image-search-build PUBLIC cxx_std_17)

