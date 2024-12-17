环境配置
========================================

跟随下列指示配置鸿蒙或安卓环境。

.. tip:: 

   环境配置步骤

   1. 确保 hdc 或 adb 命令可用

   Kea 依赖 hdc 与鸿蒙设备进行交互。 使用adb 命令与安卓设备进行交互。需要将 hdc 和 adb 命令添加到 PATH 环境变量中。

   2. 连接设备或在电脑上启动模拟器





通过 DevEco Studio 配置鸿蒙环境
---------------------------------------------------------------------


通过 Android Studio 配置安卓环境
---------------------------------------------------------------------

.. toctree:: 

   Android_Studio.rst


使用命令行配置安卓环境
-------------------------------------------------------------------

**Step 1: Install and set up android sdk on your PC**

:doc:`androidSDK/Linux`

:doc:`androidSDK/Windows`

:doc:`androidSDK/Mac`

**Setp 2: Create and run an emulator**

:doc:`androidSDK/emulator`

.. toctree::
   :hidden:
   
   androidSDK/Linux
   androidSDK/Windows
   androidSDK/Mac
   androidSDK/emulator
