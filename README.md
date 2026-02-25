## 简介
该项目fork自开源小智 [https://github.com/78/xiaozhi-esp32](https://github.com/78/xiaozhi-esp32) ，并在此基础上进行了优化和修改，主要实现自己的毕设
## 开发进度
- [2023-03-23] fork项目，并修改代码


## 遇到问题以及解决
### 项目头文件报错以及无法正常索引
    在项目根目录下创建.vscode文件夹，并在.vscode文件夹下创建c_cpp_properties.json文件，内容如下：
'''
{
    "configurations": [
        {
            "name": "ESP-IDF",
            "includePath": [
                "${workspaceFolder}/**",
                "C:/esp/v5.5.3/esp-idf/components/**"
            ]
        }
    ],
    "version": 4
}
'''