# set(<variable> <value>... [PARENT_SCOPE])
message("test set(<variable> <value>... [PARENT_SCOPE])")
set(var1 "var1")
message(${var1})

# set(<variable> <value>... CACHE <type> <docstring> [FORCE])
message("test set(<variable> <value>... CACHE <type> <docstring> [FORCE])")
set(var2 "" CACHE STRING "former var2")
message(${var2})
set(var2 "var3" CACHE STRING "this is var2")
message(${var2})
set(var2 "new var2" CACHE STRING "this is var2" FORCE)
message(${var2})
# 这个函数是给gui用的,会利用cmakecache来保存以前的值,如果不设置,则保存以前的值,设置了也没用,必须要带FORCE才可以
# 关键字大小写敏感
set(var3 "" CACHE BOOL ON)
message(INFO, ${var3})
set(var3 OFF CACHE BOOL ON)
message(INFO, ${var3})
set(var4 "" CACHE PATH "/home/kuka/")
set(var5 "" CACHE FILEPATH "/home/kuka/test")
set(var6 "" CACHE INTERNAL "internal")

# set(ENV{<variable>} <value>...)
message("set(ENV{<variable>} <value>...)")
set(ENV{var7} "var7")
#设置本进程内的参数
message("======")