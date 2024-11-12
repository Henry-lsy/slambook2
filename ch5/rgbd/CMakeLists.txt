find_package(Sophus REQUIRED)
include_directories(${Sophus_INCLUDE_DIRS} ${FMT_LIBRARIES})

find_package(Pangolin REQUIRED)

add_executable(joinMap joinMap.cpp)
target_link_libraries(joinMap ${OpenCV_LIBS} ${Pangolin_LIBRARIES} ${FMT_LIBRARIES})