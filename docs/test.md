---
layout: post
title:  "first test page"
permalink: /test/
---
# 目标
    很早以前看过 hyptertable 的实现，不是特别感兴趣，但是不看总觉得缺点什么
    目标定位在，coding sytle、设计思路、处理细节，不讨论 LSM tree 的原理这类东西

# Version

# File format
## QA
如何扩展更多的 meta block 类型
没有dio，没有对齐，对性能的影响？

## Todo
读取block时，cache相关内容没有看：Table::BlockReader
table_test.cc

## Note 
https://github.com/google/leveldb/blob/master/doc/table_format.md
记录的都是相对偏移，因此 offset 用 32位即可

## Improve
BlockBuilder：使用string进行分配，实际已经用了 tcmalloc ？