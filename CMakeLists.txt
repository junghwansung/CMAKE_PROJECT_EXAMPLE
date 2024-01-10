cmake_minimum_required(VERSION 3.13)


set(PROJECT_NAME cmake_project_example) # 변수 설정.
set(CMAKE_CXX_STANDARD 17)

project(${PROJECT_NAME})    # 
add_executable(${PROJECT_NAME} src/main.cpp)    # 두번째 인자의 것들을 컴파일해서 첫 번째 인자에 실행파일을 넣어준다.

# 1. terminal에서 실행. (OS의 빌드 시스템에 맞게 프로젝트 생성해줌.)
# cmake -Bbuild . -DCMAKE_BUILD_TYPE=Debug

# "-B" 빌드할 폴더 지정 build 라는 폴더가 생기고 거기에 
# "." CMakeLists.txt가 있는 directory 지정

# 2. terminal에서 실행. (실제 빌드)
# cmake --build build