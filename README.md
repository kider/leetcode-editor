# leetcode-editor
基于**https://github.com/shuzijun/leetcode-editor** 改造，感谢原作者，此改造版本适用于旧版本(2018+)IDEA

改动1：
增加**PackagePath**配置，用来单独配置生成代码文件的包路径。

改动2：
在**TempFilePath**配置路径后增加默认的**data**文件夹，用来存放除代码文件以外的其他临时文件。

改动3：
菜单里的全部清除不在删除PackagePath文件夹下的代码文件，只删除TempFilePath下data文件夹里的临时文件。

改动4：
选中单题清除，则清除此题的代码文件。

配置如图：
![1663859010685](https://user-images.githubusercontent.com/10611034/191784683-1bbca32c-e0ca-4052-9e2f-2e69218ef1a4.jpg)

codeTemplet配置示例：


${question.content}

package com.leetcode;

public class LeetCode$!{question.frontendQuestionId}{

    public static void main(String[] args) {
	
	Solution solution = new LeetCode$!{question.frontendQuestionId}().new Solution();
 
	}
	
	${question.code}
	
}

生成文件效果如图：

![image](https://user-images.githubusercontent.com/10611034/191785351-383edd30-6df0-487d-abf9-43f0971e806d.png)
