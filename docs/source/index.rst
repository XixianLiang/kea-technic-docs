简介
============================================================

Kea 是一个基于性质测试的工具，用于发现 Android 应用中的功能性错误。
根据一组性质，Kea 自动生成测试用例来验证这些性质。
当某个性质被违反时，Kea 会生成一个显示错误行为的错误报告。
用户可以通过以下步骤使用 Kea：

为待测应用指定性质。
性质是指应用在特定条件下的预期行为。
用户可以根据应用的规范、文档、测试用例或错误报告来指定性质。
目前，Kea 支持使用 Python 和多个 API 来指定性质。

使用指定的性质和待测应用运行 Kea。
Kea 会自动生成测试用例来探索应用。
当某个性质的前置条件满足时，Kea 会执行该性质的交互场景并检查后置条件。
如果后置条件被违反，Kea 将生成错误报告。


Contents
--------

.. toctree::
   :caption: 移动应用基于性质的测试

   part-theory/introduction

.. toctree::
   :caption: 用户手册

   part-keaUserManuel/Android_Studio
   part-keaUserManuel/first_property
   part-keaUserManuel/api
   part-keaUserManuel/tutorial
   part-keaUserManuel/options
   part-keaUserManuel/stateful testing

.. toctree::
   :caption: 用户手册

   part-designDocument/intro.rst
   
.. toctree::
   :caption: PART3: KEA FOR HarmonyOS

   part-keaForHarmonyOS/harmonyos_setup
   part-keaForHarmonyOS/harmonyos_api

.. toctree::
   :caption: PART4: APPENDIX

   part-Appendix/trophies
   part-Appendix/PDL