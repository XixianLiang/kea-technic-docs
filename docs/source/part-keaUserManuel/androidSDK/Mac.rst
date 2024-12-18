在 MAC OS 上设置 Android SDK 环境
========================================================

1. 安装 Android 命令行工具。
   前往 `Android Developer <https://developer.android.com/studio>`_ 并下载与您的操作系统匹配的工具。

   .. image::  ../../../images/android-command-line-tool.png
       :align: center

   |

   | 在这里，您可以使用 ``wget`` 下载工具，如果您愿意，也可以直接下载。

   您可以从上述 `Android Developer <https://developer.android.com/studio>`_ 网站复制下载链接。
   然后使用以下命令。

   .. code-block:: bash

       wget https://dl.google.com/android/repository/commandlinetools-mac-11076708_latest.zip?hl=zh-cn
       mkdir -p Android/cmdline-tools
       unzip commandlinetools-mac-11076708_latest.zip?hl=zh-cn -d Android/cmdline-tools
       mv Android/cmdline-tools/cmdline-tools Android/cmdline-tools/latest

2. 配置相关环境。

   安装 Java。（如果您之前已经安装并配置过，您应该检查您的 JDK 是否与命令行工具匹配，然后跳过以下关于 Java 的步骤）

   | 在这里，您可以使用 ``JDK-17`` 来匹配当前可用的最新工具。

   .. code-block:: bash

       sudo brew install openjdk@17

   打开您的 ``.bashrc`` 文件。

   .. code-block:: bash

       sudo nano ~/.zshrc

   在文件末尾添加以下内容。

   .. code-block:: bash

       export PATH="/opt/homebrew/opt/openjdk@17/bin:$PATH"
       export ANDROID_HOME="/Users/your_id_name/the_path_you_store_commandline_tools/Android"
       export PATH="$ANDROID_HOME/emulator:$ANDROID_HOME/tools:$ANDROID_HOME/cmdline-tools/latest/bin:$ANDROID_HOME/tools/bin:$ANDROID_HOME/cmdline-tools/latest:$ANDROID_HOME/platform-tools:$PATH"

   | 确保 ``PATH`` 配置与您存储相关工具的路径匹配。

   最后，重新加载 ``.zshrc`` 文件，使更改立即应用于当前终端会话。

   .. code-block:: bash

       source ~/.zshrc

3. 验证 ``sdkmanager`` 是否成功安装。

   .. code-block:: bash

       sdkmanager --update
       sdkmanager --list
       sdkmanager --licenses

   如果您获得的信息类似于以下内容，则安装成功。

   .. image::  ../../../images/sdkmanager-licenses.png
       :align: center

   |

   sdkmanager 的常用命令。您可以从 `此链接 <https://developer.android.com/tools/sdkmanager>`_ 了解更多。
