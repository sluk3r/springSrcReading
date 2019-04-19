1. xml中配置时，值都是String的， 如age=20时，xml中配置是
2. Editors: ![](/assets/editors.png)
3. PropertyEditorRegistry是管理Editor注册的入口：![](/assets/editorResitry.png)
4. TypedStringValue, 封装了这样的属性：![](/assets/typedStringValue.png), 这个类似于Hibernate中定义的各种Type:IntegerType, LongType,SetType和YesNoType等。  
   1. TypedStringValue初始化![](/assets/TypedStringValueInit.png)

   1. 初始化后，没有看到Type值![](/assets/initlizedTypedStringValue.png)

5. 这个的意思是？有什么特殊考虑？![](/assets/parseStatePushPop.png)

6. 这个好， 类似于自己设计的,ValueExtractor,从Hibernate中的String类型的Value到自己定义的ValueExtractor![](/assets/TypedStringValueInPropertyValue.png)

7. TypeDescriptor， ![](/assets/TypeDescriptor.png)
   1. 创建过程![](/assets/firstNameTypeDescriptor.png)
8. PropertyDescriptor, ![](/assets/PropertyDescriptor.png)
9. spring-framework/spring-core/src/main/java下统计Java文件， 一共有414个Java文件， 但因功能设置得当后，可以长时间大范围地复用， 价值长时间地输出。

10. 细思极恐的建模， 一个很简单的Set方法， 在这里封装成一个类， MethodParameter![](/assets/MethodParameter.png)

![](/assets/MethodParameterDef.png)









