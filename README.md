# Python_1+X 职业技能等级考试_助教(大语言模型)


主要用于职业院校考取中慧云启的Python_1+x职业技能等级证书的考题解答和咨询。😊  
这里面包含问答题的源码、模拟题答案详解，以及考核标准的解读。  
 

#


![image](https://github.com/mmb135/python_tutor/assets/156198133/799122b6-cc55-437a-9637-ad99d13a531f)
#

![image](https://github.com/mmb135/python_tutor/assets/156198133/ab0f6b5f-9128-4b62-9b3a-820778102a2e)

#
![image](https://github.com/mmb135/python_tutor/assets/156198133/4b6bace5-8568-4793-87d1-6e8678163fe5)


#
教材选用

![image](https://github.com/mmb135/python_tutor/assets/156198133/8995537c-9ca1-4272-8371-88679396650b)



##创建conda环境
1.安装
~~~
pip install xtuner
~~~
#
2.挑选配置模板
~~~
xtuner list-cfg -p internlm_20b
~~~
3.一键训练
~~~
xtuner train internlm_20b_qlora_oasst1_512_e3
~~~
4.config命名规则
模型名 internlm_20b  无chat代表时基座模型
使用算法 qlora
数据集 oasst1
数据长度 512
Epoch e3,epoch3
![image](https://github.com/mmb135/python_tutor/assets/156198133/459eeed1-50b5-418c-9c1c-ffa77694a294)

##自定义训练
1.拷贝配置模板
~~~
xtuner copy-cfg internlm_20b-qlora_oasst1_512_e3 ./
~~~
2.修改配置模板
~~~
vi internlm_20b_qlora_oasst1_512_e3_copy.py
~~~
3.启动训练
xutner train internlm_20b_qlora_oasst1_512_e3_copy.py







