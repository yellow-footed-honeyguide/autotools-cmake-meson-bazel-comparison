# Autotools vs CMake vs Meson vs Bazel

## Projects

| Makefile Only | CMake (2000) | Autotools (1991) | Meson (2013) | Bazel (2015) |
|---------------|--------------|------------------|--------------|--------------|
| agda (2005) | CMake (2000) | autoconf (1991) | Hyprland (2022) | bazel (2015) |
| alacritty (2016) | Halide (2012) | bash (1989) | Marker (2018) | chapel (2009) |
| autojump (2008) | Hyprland (2022) | bazel (2015) | arrow (2016) | cockroach (2015) |
| bokeh (2012) | Idris-dev (2009) | binutils (1988) | budgie-desktop (2013) | envoy (2016) |
| cassandra (2008) | arrow (2016) | caja (2012) | foot (2019) | fuchsia (2016) |
| cli (N/A) | avro (2009) | cava (2016) | fuchsia (2016) | gecko-dev (1998) |
| clib (2013) | bat (2018) | chapel (2009) | gecko-dev (1998) | kubernetes (2014) |
| cmus (2005) | bazel (2015) | cpython (1991) | gnome-shell (2008) | llvm-project (2003) |
| coq (1989) | binutils (1988) | curl (1997) | gnome-terminal (2002) | moby (2013) |
| dask (2014) | calibre (2006) | gcc (1987) | grim (2018) | mongo (2009) |
| dmd (2001) | cava (2016) | gecko-dev (1998) | gstreamer (2001) | pytorch (2016) |
| docker-ce (2013) | ceph (2006) | git (2005) | i3 (2009) | rabbitmq-server (2007) |
| druid (2012) | chapel (2009) | linux (1991) | matplotlib (2003) | sdk (N/A) |
| dua-cli (2019) | cmark-gfm (2017) | llvm-project (2003) | meson (2013) | tensorflow (2015) |
| dwm (2006) | cpython (1991) | lxpanel (2006) | mongo (2009) | |
| elixir (2011) | curl (1997) | lxterminal (2008) | mpv (2013) | |
| fd (2017) | fish-shell (2005) | mate-panel (2011) | mutter (2001) | |
| flink (2014) | gcc (1987) | mesos (2009) | nautilus (1999) | |
| frege (2011) | gecko-dev (1998) | mongo (2009) | pandas (2008) | |
| fsharp (2005) | git (2005) | nano (1999) | pipewire (2017) | |
| fzf (2013) | gpdb (2016) | ncdu (2007) | postgres (1996) | |
| gensim (2009) | gstreamer (2001) | ocaml (1996) | rofi (2012) | |
| gitui (2020) | hadoop (2006) | otp (1986) | scikit-learn (2007) | |
| glow (2019) | hbase (2008) | pcmanfm (2006) | scipy (2001) | |
| go (2009) | ignite (2014) | php-src (1995) | slurp (2018) | |
| gosu-lang (2009) | keepassxc (2016) | postgres (1996) | sway (2016) | |
| ipython (2001) | kwin (1999) | rofi (2012) | systemd (2010) | |
| jaeger (2016) | linux (1991) | ruby (1995) | tokei (2015) | |
| julia (2012) | lldb (2010) | rufus (2011) | vlc (2001) | |
| kivy (2011) | llvm-project (2003) | sqlite (2000) | xfdesktop (2002) | |
| lazydocker (2019) | meson (2013) | storm (2011) | xserver (1984) | |
| lazygit (2018) | mesos (2009) | tarantool (2010) | | |
| lfe (2008) | mongo (2009) | tesseract (2006) | | |
| minio (2014) | neovim (2014) | the_silver_searcher (2011) | | |
| navi (2019) | ninja (2010) | thrift (2007) | | |
| neofetch (2015) | obs-studio (2012) | thunar (2004) | | |
| newsboat (2017) | opencv (2000) | vim (1991) | | |
| nnn (2016) | orc (2008) | vlc (2001) | | |
| notebook (2015) | ponyc (2015) | wget (1996) | | |
| ohmyzsh (2009) | pytorch (2016) | xfdesktop (2002) | | |
| parquet-format (2013) | rustdesk (2020) | xfwm4 (2002) | | |
| plotly.py (2013) | rustdesk (2020) | zookeeper (2008) | | |
| powerlevel10k (2018) | tarantool (2010) | zsh (1990) | | |
| procs (2019) | tensorflow (2015) | | | |
| purescript (2013) | tesseract (2006) | | | |
| ranger (2009) | thrift (2007) | | | |
| runit (2001) | tvm (2017) | | | |
| s6 (2004) | vlc (2001) | | | |
| spaCy (2015) | yugabyte-db (2016) | | | |
| spark (2009) | zig (2015) | | | |
| sysvinit (1983) | zookeeper (2008) | | | |
| tikv (2016) | | | | |
| transformers (2018) | | | | |
| v (2019) | | | | |
| vitess (2010) | | | | |
| wttr.in (2016) | | | | |
| z (2009) | | | | |


## Makefile depend on system

a) Commands and utilities:
Linux:
```makefile
RM = rm -f
```
Windows:
```makefile
RM = del /Q
```

b) File paths:
Linux:
```makefile
INCLUDE_DIR = /usr/local/include
```
Windows:
```makefile
INCLUDE_DIR = C:\Program Files\include
```

c) Executable file extensions:
Linux:
```makefile
TARGET = myprogram
```
Windows:
```makefile
TARGET = myprogram.exe
```

d) Compilers and flags:
Linux (GCC):
```makefile
CC = gcc
CFLAGS = -Wall -O2
```
Windows (MSVC): 
```makefile CC = cl CFLAGS = /W3 /O2 ```


## Perfomance


| Place | Tool | Reward |
|-------|------------|---------|
| 1     | Bazel      | 🏆🏆🏆   |
| 2     | Meson      | 🏆🏆    |
| 3     | CMake      | 🏆      |
| 4     | Autotools  |         |

## Documentation

| Place | Tool | Reward |
|-------|------------|---------|
| 1     | Meson      | 🏆🏆🏆   |
| 2     | CMake      | 🏆🏆    |
| 3     | Bazel      | 🏆     |
| 4     | Autotools  |        |







## Build Systems Comparison

| Aspect | Autotools | CMake | Meson | Bazel |
|--------|-----------|-------|-------|-------|
| Language | Shell scripts & M4 macros. Very slow. | C++. Faster than Autotools, but not blazing fast. | Python. Fast if well-written. | Java (core) + Starlark (configs). Verbose but fast. |
| Caching | Poor. config.cache exists but ineffective. | Better. CMakeCache.txt remembers some things. | Good. Stores intermediate results efficiently. | Excellent. Distributed caching, incremental builds. |
| Parallelization | No native support. Relies on make -j. | Built-in support, but not very smart. | Out of the box, works well. | Advanced. Capable of distributed builds. |
| Config Parsing | Very slow. New process for each check. | Moderate. Custom CMakeLists.txt, parses faster than Autotools. | Fast. Custom DSL based on Python - parses quickly. | Fast. Starlark (simplified Python) parses quickly. |
| Summary | Old reliable. Trusted but slow. | Workhorse. Not flashy, but gets the job done. | Young and fast. Modern, quick, but not universally adopted. | Corporate powerhouse. Powerful, fast, but complex to learn. |

Note: Even with the most advanced build system, poor configuration can result in slow build times.




## Build Systems Languages
| Task | Autotools | CMake | Meson | Bazel |
|------|-----------|-------|-------|-------|
| 1. Simple compilation and linking | configure.ac:<br>```AC_INIT([myapp], [1.0])<br>AM_INIT_AUTOMAKE<br>AC_PROG_CC<br>AC_CONFIG_FILES([Makefile])<br>AC_OUTPUT```<br><br>Makefile.am:<br>```bin_PROGRAMS = myapp<br>myapp_SOURCES = main.c``` | ```cmake_minimum_required(VERSION 3.10)<br>project(myapp)<br>add_executable(myapp main.c)``` | ```project('myapp', 'c')<br>executable('myapp', 'main.c')``` | ```cc_binary(<br>    name = "myapp",<br>    srcs = ["main.c"],<br>)``` |
| 2. Adding an external library (e.g., libxml2) | configure.ac:<br>```PKG_CHECK_MODULES([XML], [libxml-2.0])```<br><br>Makefile.am:<br>```myapp_CFLAGS = $(XML_CFLAGS)<br>myapp_LDADD = $(XML_LIBS)``` | ```find_package(LibXml2 REQUIRED)<br>target_link_libraries(myapp LibXml2::LibXml2)``` | ```xml_dep = dependency('libxml-2.0')<br>executable('myapp', 'main.c', dependencies: xml_dep)``` | ```cc_binary(<br>    name = "myapp",<br>    srcs = ["main.c"],<br>    deps = ["@libxml2//:libxml2"],<br>)``` |
| 3. Setting installation directory | configure.ac:<br>```AC_PREFIX_DEFAULT(/usr/local)``` | ```set(CMAKE_INSTALL_PREFIX /usr/local)``` | ```project('myapp', 'c', default_options: ['prefix=/usr/local'])``` | No direct equivalent. Custom installation rules needed. |
| 4. Adding a custom compiler | configure.ac:<br>```AC_PROG_CC([clang gcc])``` | ```set(CMAKE_C_COMPILER clang)``` | ```project('myapp', 'c', default_options: ['c_compiler=clang'])``` | In WORKSPACE file:<br>```load("@bazel_tools//tools/cpp:cc_configure.bzl", "cc_configure")<br>cc_configure(cc_path = "/path/to/clang")``` |
| 5. Creating and running tests | Makefile.am:<br>```TESTS = test1 test2<br>check_PROGRAMS = test1 test2<br>test1_SOURCES = test1.c<br>test2_SOURCES = test2.c``` | ```enable_testing()<br>add_executable(test1 test1.c)<br>add_executable(test2 test2.c)<br>add_test(NAME Test1 COMMAND test1)<br>add_test(NAME Test2 COMMAND test2)``` | ```test('test1', executable('test1', 'test1.c'))<br>test('test2', executable('test2', 'test2.c'))``` | ```cc_test(<br>    name = "test1",<br>    srcs = ["test1.c"],<br>)<br>cc_test(<br>    name = "test2",<br>    srcs = ["test2.c"],<br>)``` |



## Comparison of abstraction level

### 1. Simple Compilation and Linking

#### Autotools

```autotools
# configure.ac:
AC_INIT([myapp], [1.0])
AM_INIT_AUTOMAKE
AC_PROG_CC
AC_CONFIG_FILES([Makefile])
AC_OUTPUT

# Makefile.am:
bin_PROGRAMS = myapp
myapp_SOURCES = main.c
```

#### CMake

```cmake
cmake_minimum_required(VERSION 3.10)
project(myapp)
add_executable(myapp main.c)
```

#### Meson

```meson
project('myapp', 'c')
executable('myapp', 'main.c')
```

#### Bazel

```python
cc_binary(
    name = "myapp",
    srcs = ["main.c"],
)
```

## 2. Adding an External Library (e.g., libxml2)

#### Autotools

```autotools
# configure.ac:
PKG_CHECK_MODULES([XML], [libxml-2.0])

# Makefile.am:
myapp_CFLAGS = $(XML_CFLAGS)
myapp_LDADD = $(XML_LIBS)
```

#### CMake

```cmake
find_package(LibXml2 REQUIRED)
target_link_libraries(myapp LibXml2::LibXml2)
```

#### Meson

```meson
xml_dep = dependency('libxml-2.0')
executable('myapp', 'main.c', dependencies: xml_dep)
```

#### Bazel

```python
cc_binary(
    name = "myapp",
    srcs = ["main.c"],
    deps = ["@libxml2//:libxml2"],
)
```

### 3. Setting Installation Directory

#### Autotools

```autotools
# configure.ac:
AC_PREFIX_DEFAULT(/usr/local)
```

#### CMake

```cmake
set(CMAKE_INSTALL_PREFIX /usr/local)
```

#### Meson

```meson
project('myapp', 'c', default_options: ['prefix=/usr/local'])
```

#### Bazel

Bazel doesn't have a direct equivalent. Custom installation rules are needed.

### 4. Adding a Custom Compiler

#### Autotools

```autotools
# configure.ac:
AC_PROG_CC([clang gcc])
```

#### CMake

```cmake
set(CMAKE_C_COMPILER clang)
```

#### Meson

```meson
project('myapp', 'c', default_options: ['c_compiler=clang'])
```

#### Bazel

```python
# In WORKSPACE file:
load("@bazel_tools//tools/cpp:cc_configure.bzl", "cc_configure")
cc_configure(cc_path = "/path/to/clang")
```

### 5. Creating and Running Tests

#### Autotools

```autotools
# Makefile.am:
TESTS = test1 test2
check_PROGRAMS = test1 test2
test1_SOURCES = test1.c
test2_SOURCES = test2.c
```

#### CMake

```cmake
enable_testing()
add_executable(test1 test1.c)
add_executable(test2 test2.c)
add_test(NAME Test1 COMMAND test1)
add_test(NAME Test2 COMMAND test2)
```

#### Meson

```meson
test('test1', executable('test1', 'test1.c'))
test('test2', executable('test2', 'test2.c'))
```

#### Bazel

```python
cc_test(
    name = "test1",
    srcs = ["test1.c"],
)
cc_test(
    name = "test2",
    srcs = ["test2.c"],
)
```

## Systemd Syntax

| Meson Construct | Description |
|-----------------|-------------|
| project() | Defines the project name, language, and version. |
| set_default() | Sets a default value for an option. |
| add_project_arguments() | Adds compiler arguments for the entire project. |
| add_project_link_arguments() | Adds linker arguments for the entire project. |
| configuration_data() | Creates an object to store configuration data. |
| set() | Sets a value in the configuration_data object. |
| set10() | Sets a boolean value (0 or 1) in the configuration_data object. |
| set_quoted() | Sets a quoted string value in the configuration_data object. |
| import() | Imports a Meson module. |
| find_program() | Searches for an executable file in the system. |
| run_command() | Executes an external command. |
| dependency() | Declares a dependency on an external library. |
| declare_dependency() | Creates a dependency object. |
| include_directories() | Adds directories for header file searches. |
| files() | Creates a list of files. |
| configure_file() | Generates a file based on a template. |
| custom_target() | Creates a custom build target. |
| executable() | Creates an executable file. |
| shared_library() | Creates a shared library. |
| static_library() | Creates a static library. |
| test() | Declares a test. |
| install_data() | Installs data files. |
| install_headers() | Installs header files. |
| install_man() | Installs man pages. |
| install_subdir() | Installs a subdirectory. |
| foreach | Loop for iterating over a list. |
| if/elif/else | Conditional constructs. |
| and/or/not | Logical operators. |
| error() | Outputs an error message and halts execution. |
| warning() | Outputs a warning message. |
| message() | Outputs a message. |
| summary() | Outputs a configuration summary. |
| subdir() | Enters a subdirectory and executes the meson.build there. |
| get_option() | Gets the value of a build option. |
| host_machine | Object for obtaining information about the target system. |
| meson | Global object with project information and methods. |
| fs | Module for working with the file system. |
| cc | Compiler object. |
| run_target() | Creates a target that can be run manually. |
| alias_target() | Creates an alias for another target. |
| generator() | Creates a generator for automatic source file creation. |






## Turing Completeness of Build System Configuration Languages
| Build System | Turing Complete | Proof/Explanation |
|--------------|-----------------|-------------------|
| Autotools    | Partially       | Autotools uses M4 (not Turing-complete) and shell scripts (Turing-complete). M4 itself lacks unbounded loops. Shell example: `factorial() { [ $1 -le 1 ] && echo 1 || echo $(( $1 * $(factorial $(( $1 - 1 ))) )); }` |
| CMake        | True            | CMake supports recursion and unbounded loops. Factorial example: `function(factorial n result) if(${n} LESS 2) set(${result} 1 PARENT_SCOPE) else(math(EXPR n1 "${n} - 1") factorial(${n1} sub_result) math(EXPR res "${n} * ${sub_result}") set(${result} ${res} PARENT_SCOPE)) endif() endfunction()` |
| Meson        | False           | Meson intentionally limits looping and recursion for predictability. It lacks unbounded loops and general recursion. This factorial won't work: `def factorial(n): return 1 if n <= 1 else n * factorial(n - 1)` |
| Bazel        | False           | Bazel's Starlark is intentionally not Turing-complete. It disallows recursion and while loops. This factorial function is not possible: `def factorial(n): return 1 if n <= 1 else n * factorial(n - 1)` |
