Kea 技术文档
=======================================

https://kea-technic-docs.readthedocs.io/zh-cn/latest/

开发者指南
======================================

**1.初始化**

.. code-block:: bash

    git clone git@github.com:XixianLiang/kea-technic-docs.git

    cd kea-technic-docs/docs

    pip install -r requirements.txt


**2.使用 vscode RST 预览器**

添加下列vscode拓展:

`reStructuredText <https://marketplace.visualstudio.com/items?itemName=lextudio.restructuredtext>`_

`reStructuredText Syntax highlighting <https://marketplace.visualstudio.com/items?itemName=trond-snekvik.simple-rst>`_

`Esbonio <https://marketplace.visualstudio.com/items?itemName=swyddfa.esbonio>`_

安装 Esbonio 服务器

.. code-block:: bash
    
    pip install esbonio

重启vscode

**3. Build html**

.. code-block:: bash

    cd kea-technic-docs/docs

    # You should delete the build dir every time you modify the file structure of the project
    # Or the cache will affect the previewer of the esbonio extension.
    rm -r build

    make html


Template for the Read the Docs tutorial
=======================================

This GitHub template includes fictional Python library
with some basic Sphinx docs.

Read the tutorial here:

https://docs.readthedocs.io/en/stable/tutorial/
