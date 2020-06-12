# get_target_property(VAR target property)
#[[get_property(<variable>
<GLOBAL             |
DIRECTORY [dir]    |
TARGET    <target> |
SOURCE    <source> |
INSTALL   <file>   |
TEST      <test>   |
CACHE     <entry>  |
VARIABLE>
PROPERTY <name>
[SET | DEFINED | BRIEF_DOCS | FULL_DOCS])
]]
#[[set_target_properties(target1 target2 ...
                      PROPERTIES prop1 value1
                      prop2 value2 ...)
]]
#[[define_property(<GLOBAL | DIRECTORY | TARGET | SOURCE |
                 TEST | VARIABLE | CACHED_VARIABLE>
                 PROPERTY <name> [INHERITED]
                 BRIEF_DOCS <brief-doc> [docs...]
                 FULL_DOCS <full-doc> [docs...])
]]

#TODO language variable and cache variable

#set_property(<GLOBAL                         |
#              DIRECTORY [dir]                   |
#              TARGET    [target1 [target2 ...]] |
#              SOURCE    [src1 [src2 ...]]       |
#              INSTALL   [file1 [file2 ...]]     |
#              TEST      [test1 [test2 ...]]     |
#              CACHE     [entry1 [entry2 ...]]>
#             [APPEND] [APPEND_STRING]
#             PROPERTY <name> [value1 [value2 ...]])
message("======")
