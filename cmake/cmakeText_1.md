写一个简单的`CMake`模板
```c++
# 设置当前 cmake 版本信息
cmake_minimum_required(VERSION 3.5)

# 这里可以设置项目名称
project(Pro1_1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 添加项目
add_executable(Pro1_1 main.cpp)

```
当然，我们也可以使用`set(set是为设置一个变量)`替换 `main.cpp`
使用`set`替换后如下
```c++

cmake_minimum_required(VERSION 3.5)

project(Pro1_1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
# 如果在windows 平台，加上 WIN32 可以去掉黑色框
set(EXC WIN32
	mian.cpp
)

add_library(GLFW)

add_executable(EXC main.cpp)

```
