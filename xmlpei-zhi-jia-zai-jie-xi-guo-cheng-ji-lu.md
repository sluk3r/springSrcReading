1. 入口测试类![](/assets/入口测试类.png)
2. static地先加载下类。先快速解决，而不考虑优雅 ![](/assets/static_load_class.png)
3. PathMatchingResourcePatternResolver下的equinoxResolveMethod加载，

    ![](/assets/equinoxResolveMethod_prepare.png)

4. 关于PathMatcher， 默认是这个AntPathMatcher， 看PathMatcher的抽象方式，isPattern，match，matchStart，extractPathWithinPattern，extractUriTemplateVariables，getPatternComparator，combine。

5. 不单单是表面上的一对一， 而是通过规则的一对多。 ![](/assets/pattern_resolver.png)

6. 关于parentContext, 看到做的事， 只是merge下Environment![](/assets/mergeEnvironment.png)

7. 文件名上的规则,这个是不是profile魔力发生的地方？![](/assets/file_name_rule.png)

8. 什么情况下， 不需要refresh呢？ ![](/assets/when_not_refresh.png)

9. 关于配置， 不是在编译器写好后， 再靠各种开关控制着某些特性的启用。 而现在靠恰当的接口或类继承后， 再在使用时， API地选出来合适的组合。

10. 又是一个加载类的方式![](/assets/another_class_loader_example.png)

11. InternalParentBeanFactory对应的场景？![](/assets/internalParentBeanFactory.png)

12. ClassPathXmlApplication**Context**,AbstractXmlApplication**Context**,AbstractRefreshableConfigApplication**Context**,AbstractRefreshableApplication**Context**,AbstractApplication**Context**![](/assets/contexts.png)

13. ParentBeanFactory， ![](/assets/setParentBeanFactory.png)

14. 创建BeanFactory后， 把定制化的工作， 留给子类，

15. 在finishBeanFactoryInitialization方法里再通过preInstantiateSingletons， 触发单例对象的生成。

16. isAbstract, isSingleton, isLazyInit![](/assets/abstract-singleton-lazyInit.png)

17. MergedBeanDefinition,Return a RootBeanDefinition for the given bean, by merging with the parent if the given bean's definition is a child bean definition.

18. before-do-after, 很常见的套路![](/assets/before-do-after.png)

19. 这个singletonFactory的调用只是一个HappyPath： ![](/assets/create_happy_path.png)

20. 关于synthetic， 看描述， 是not defined by the application itself.看来，Spring内部有判断， 什么情况下的Bean有设置这个呢？![](/assets/bean-synthetic.png)

21. 内部定义了一个专门的接口， PropertyValues， 这个更高级的管理方式，还是第一次见。 从List到List的简单封装， 再到接口封装PropertyValues，看到进一步的抽象。 今天可就这个话题写一篇博客。 ![](/assets/PropertyValues.png)

22. 越看越觉得， 类似于实现了一个Mysql这样大的系统，从最原生的地方同步概念。一层一志勇的概念搭建。![](/assets/atom_concept.png)

23. value Resolve, 是不是指placeHolder?![](/assets/TypedStringValue.png)



