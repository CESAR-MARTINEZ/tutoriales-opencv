cmake_minimum_required(VERSION 3.4)

project( AcentuarColor )

find_package( OpenCV 3.0.0 REQUIRED )

file(COPY ../data/messi.jpg DESTINATION image)

add_executable( ${PROJECT_NAME} source.cpp )
target_link_libraries( ${PROJECT_NAME} ${OpenCV_LIBS} )