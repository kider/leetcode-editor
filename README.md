# leetcode-editor
基于**https://github.com/shuzijun/leetcode-editor** 改造，感谢作者的开源，此改造版本适用于旧版本(2018+)IDEA

改动1：
增加PackagePath配置，用来单独配置生成代码文件的包路径。

改动2：
在TempFilePath配置路径后增加默认的data文件夹，用来存放除代码文件以外的其他临时文件。

改动3：
菜单里的全部清除不在清除包含PackagePath文件夹下的代码文件，只清除TempFilePath下的data文件夹的临时内容。

改动4：
选中单题清除，则清除此题的代码文件。
