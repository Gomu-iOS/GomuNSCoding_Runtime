# GomuNSCoding_Runtime

归档解档
归档和解档需要对每个属性都实现一遍encodeObject:forKey:和decodeObjectForKey:方法，这样就会显得比较繁琐，但是我们可以利用Runtime获取所有属性来重写归档解档方法。

创建一个NSObject的分类@interface NSObject (Runtime)：

![image]()
