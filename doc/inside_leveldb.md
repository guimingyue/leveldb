`void Version::ForEachOverlapping(Slice user_key, Slice internal_key, void* arg,
                                 bool (*func)(void*, int, FileMetaData*))`
先查找 level 0，level 0 的文件会按照先后顺序（FileMetaData.number的大小）排序，再从新往旧查找。
level 0 查找完成后，再查找 level 1 


# 问题
level 0 的文件有什么特征？相对于其他 level 有什么区别？
