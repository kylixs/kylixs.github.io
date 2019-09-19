20190919 Rust性能优化技巧 

1、整数转换为字符串（int to str）  

  itoa 性能远高于Rust int.to_string()

2、Vec.set_len() 性能比 Vec.resize() 好得多

3、Vec< i64 >与Vec< u8 >互相转换


4、BufReader性能不是很好，大量创建小对象

5、serde_json性能不错，比resp性能还要好



