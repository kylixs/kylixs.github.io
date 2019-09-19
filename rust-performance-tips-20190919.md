20190919 Rust性能优化技巧 

1、整数转换为字符串（int to str）  

  itoa 性能远高于Rust int.to_string()

2、Vec.set_len() 性能比 Vec.resize() 好得多

3、Vec< i64 >与Vec< u8 >互相转换


4、BufReader性能不是很好，大量创建小对象

5、serde_json性能不错，比resp性能还要好   
思考：更快但方便兼容新旧版本的二进制序列化方法
1）参考resp的思想，改为二进制方式   
```
   data type (1 byte)| data content(n bytes) 
   type: i32 (1 byte)| data content(4 bytes) 
   type: i64 (1 byte)| data content(8 bytes) 
   type: short string (1 byte)| len (2 bytes) | data content(n bytes) 
   type: long string (1 byte)| len (4 bytes) | data content(n bytes) 
   type: array (1 byte)| len (2 bytes) | data content(n bytes) 
   ...
```


