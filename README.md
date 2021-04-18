# HNU-AutoClockIn

湖大疫情防控自动打卡脚本 ( github action )

采用提交请求方式进行打卡，github action自动运行

默认时间为凌晨1点和早上6点各三次（防止github action虚拟器未构建成功）

此外，该脚本已经运行直到**打卡成功** 或者 **达到github action上限运行时间（6小时）**

所以如果没有收到github给你发的**action报错邮件**就说明打卡成功

# 使用手册

先fork本仓库，然后在自己的仓库中进行设置

请在仓库设置中的`secret`项打入如下键值对

| 键                       | 值                                              |
| ------------------------ | ----------------------------------------------- |
| USER                     | 学号                                            |
| PASSWORD                 | 密码                                            |
| REALPROVINCE_CITY_COUNTY | 例如： 湖南省,长沙市,岳麓区（请用英文逗号隔开） |
| REALADDRESS              | 具体地址                                        |

点击仓库star可以手动运行，在action里可以看历史运行结果

# 免责声明

请在法律循序范围内使用，当发生发烧等异常现象是仍需如实填报。若用户使用此脚本后违反相关法律法规造成损失，将由用户自行承担，作者不承担一切责任！

