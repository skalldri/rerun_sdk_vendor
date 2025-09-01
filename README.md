# rerun_sdk_vendor

This ROS2 package makes the ReRun C++ SDK available to other packages.

## Usage

In `package.xml`:

```
<depend>rerun_sdk_vendor</depend>
<depend>rerun_sdk</depend>
```

In CMakeLists.txt:

```
find_package(rerun_sdk_vendor REQUIRED)
find_package(rerun_sdk REQUIRED)

# ...

target_link_libraries(my_target PRIVATE rerun_sdk)
```
