# 第一天源码研读记录

## 版本
- 我的 Fork 地址：https://github.com/thy11111/learn-claude-code
- 官方源码目录：C:\Users\15955\AgentStudy\learn-claude-code
- 本日练习目录：C:\Users\15955\AgentStudy\Day1_Agent_Study
- Conda 环境：agent_harness
- SDK base_url：https://api.siliconflow.cn/v1
- 上游 commit：
- 学习日期：
- 我使用的 Python 版本与解释器：

## 入口与两个循环
- CLI 入口函数或代码位置：
- 外层循环一轮代表：
- 内层循环一轮代表：
- 两个循环的退出条件：

## 消息快照
写出 A 用户输入、B 工具请求、C 工具结果、D 最终回答的消息角色与关键字段。

## 工具调用链
用自己的话写出 main 到 generate 到 dispatch 到 read_file 再回到 generate 的过程。

## 运行记录
| 场景 | 模型请求次数 | 历史条数 | 停止状态 | 观察 |
| --- | --- | --- | --- | --- |
| normal | | | | |
| multiple | | | | |
| recover | | | | |
| endless max 3 | | | | |
| SiliconFlow 真模型 | | | | |

## 真实模型协议转换
- 我实际使用的模型 ID（不要记录密钥）：
- input_schema 到 function.parameters：
- tool_use 到 tool_calls：
- tool_result 到 role=tool：
- 为什么工具参数需要 json.loads：
- smoke 成功能验证什么，不能验证什么：
- 第二次 API 请求里实际包含了什么文件结果：

## 设计问题
- Schema 与 handler 有什么区别：
- 为什么结果要带 ID：
- 为什么要保存 assistant 调用：
- FakeLLM 能验证什么：
- 两项上游边界或我的改进：

## 自测薄弱项
- 题号：
- 我的原答案：
- 修正后的解释：

## 今日改动与验证
- 我独立修改了什么：
- 测试结果：
- 明天需要实现什么：


两个循环的职责。
A、B、C、D 四个消息时刻。
工具调用 ID 与结果 ID 的配对。
Schema、Dispatcher、handler 的区别。
正常、多工具、错误恢复和超限场景的观察。
使用的真实模型 ID。
第二次模型请求中包含的工具结果。
仍未解决的问题