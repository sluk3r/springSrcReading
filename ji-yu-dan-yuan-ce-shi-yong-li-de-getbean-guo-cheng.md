1. 入口类：  
   ![](/assets/entry.png)

2. ResourcePatternResolver的必要性![](/assets/patternResolver.png)

3. 如果形容人的话， 很真的是很懒， 只有在真正使用时， 才创建：![](/assets/lazyCreate.png)

4. 跟人类社会里的组织协调工作一样， 组织协调工作都是重点和难点： ![](/assets/zuzhiXietiao.png)

5. 文件名上也可以按某种规则替换？![](/assets/fileNameReplace.png)

6. 使用的是ConfigurableListableBeanFactory![](/assets/obtainConfigurableListableBeanFactory.png)

7. javaxInjectProviderClass是能啥的？ 是为让非Spring的实现注入进来？![](/assets/javaxInjectProviderClass.png)

8. 看到跟自己设计思路很相近的地方， 接口实现里， 添加特定的实现类Delegate![](/assets/design_echo.png)

9. EntityResolver是org.xml.sax中的定义， 它在Xml解析过程中的价值，后面再系统性地梳理![](/assets/ResourceEntityResolver.png)

10. 先init再真正地load,![](/assets/initThenLoad.png), 看注释很有同感。

11. 一个locationPattern返回Resource\[\], ![](/assets/locationPattern-multi-Resource.png)

12. 自带的PathMatcher实现类中只有AntPathMatcher， 暂没有别的实现。

13. Context是一个重要的理念， 不单单像Map一样， 也可以往Context中放使用到的引用，![](/assets/ReaderContext.png)

14. Delegate是真正干活的，这个很正常，外面都被协调给包围了 ![](/assets/delegate.png)这个类是Stateful的考虑是？ 

15. 


