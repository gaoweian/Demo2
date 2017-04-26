# Hashtable和HashMap的区别
* Hashtable:实现的是映像，不允许出现空键空值，线程安全，现已被HashMap替代。
* HashMap：实现一个键到值映射的哈希表，通过get()获得value()，允许出现空键空值(因键的值是唯一的),线程不安全。
# 在try中加return会走finally吗？
```
    public class Demo{
	public static void main(String[] args){
		int a=0,b=2,c;
		try{
			c=a/b;
			return ;
		}catch (Exception e) {
				e.printStackTrace();
		}finally{
			System.out.println("出口");
		}
	}
}
```
* 会走
  
# ArrayList和LinkedList区别：
* 实现一个数组，可以快速存取。
* 实现一个链表，可以快速插入和移除数据。
# StringBuffer和StringBuilder区别：
* StringBuffer:StringBuffer是可变类，任何对它所指代的字符串的改变都不会产生新的对象。线程安全，适合多线程使用。
* StringBuilder:在进行append时，选择StringBuffer。线程不安全，适合单线程使用。

