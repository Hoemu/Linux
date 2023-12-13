# 写一个简单的`CMake`模板
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

# 导入外部库文件
```c++
include_directories(${FilePath})/// 导入头文件
link_directores(${})		/// 导入库文件目录到当前工程
link_libraries(${lib.a})	/// 导入库文件到当前工程
target_link_libraries()		/// 导入库文件到子工程
target_include_directories()	/// 导入头文件目录到子工程

```

## 如何导入一个 `OpenCV` 库？
下面代码生效的前提是已经生成了`OpenCV`的`Build`
```c++
find_package(OpenCV 4.5 REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(PorjectName ${OpenCV_LIBS})

```
### 如果出现`cmake`出现异常情况，则检查一下环境是否配置
```c++
/// 标准环境路径
D:\***\****\opencv-build\bin
```
