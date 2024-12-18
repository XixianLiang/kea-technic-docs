keaTestElements
=========================

keaTestElements与用户继承并自定义的keaTest一一对应。在kea运行时，keaTestElements会读取每个用户自定义的keaTest，
并重新组织为方便kea进行读取的数据结构。具体转换过程可参考：:ref:`decorators-keatestelements`。


keaTestElements的数据结构和成员方法定义如下：

.. code-block:: python

    class KeaTestElements:
        self.keaTest_name: str
        self.rules: List[Rule]
        self.initializers: List[Initializer]
        self.mainPaths: List[MainPath]

        def load_rules(keaTest)
        def load_initializers(keaTest)
        def load_mainPaths(keaTest)