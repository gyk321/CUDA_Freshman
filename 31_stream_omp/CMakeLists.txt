find_package(OpenMP REQUIRED)

add_executable(stream_omp stream_omp.cu)
target_compile_options(stream_omp PRIVATE -Xcompiler=-fopenmp)
target_link_libraries(stream_omp PRIVATE OpenMP::OpenMP_CXX)

