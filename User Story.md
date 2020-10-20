User Story

一
简答题

1
用自己的话描述什么是用户故事。（15分）
答：
书面的需求描述，完整记录需求内容与功能细节，通常以卡片形式呈现。提供了关于需求不同角色间对话的依据，具体化需求细节。定义需求是否完成的判断标准，定义了需求细节，对每个细节定义验收标准。

2
用户故事的3Cs是什么？（10分）
答：
Card，Conversation，Confirmation。

3
一个用户故事一般包含哪些内容？并简述每一部分内容。（20分）
答：
包括概览与详情。
概览，一般只包含用户故事标题与创建编号。
详情，包括需求描述、验收标准、附件等。需求描述，概述整个故事，As用户角色，I want需求，So that业务价值。验收标准，定义需求细节以及如何验收该需求，定义需求范围与边界，给定了需求完成的定义。附件，可能根据需要包含原型图、数据样例等。

4
什么是Acceptance Criteria？（15分）
答：
验收标准，定义需求细节以及如何验收该需求，定义需求范围与边界，给定了需求完成的定义。格式，Given需求前置条件或定义需求发生场景，When描述当前需求场景何时出现，Then描述需求场景发生时表现。一个用户故事可有多个AC，每个AC对于一个需求场景，一般分为三类，正常情况，系统异常情况，正常情况下其他相关需求。

二
情景题

根据以下需求，写出Acceptance Criteria。（40分）
As a ThoughtWorker
I want to order coffee using coins
So that I can stay awake during sessions
答：

AC1:
Given
我是一名ThoughtWorker。
And
我持有等于一杯咖啡价格的硬币。
When
我给出硬币点一杯咖啡。
Then
我可以获得一杯咖啡。

AC2:
Given
我是一名ThoughtWorker。
And
我持有高于一杯咖啡价格的硬币。
When
我给出硬币点一杯咖啡。
Then
我可以获得一杯咖啡。
And
系统退回多余硬币。

AC3:
Given
我是一名ThoughtWorker。
And
我持有等于一杯咖啡价格的硬币。
And
系统发生故障无法给出咖啡。
When
我给出硬币点一杯咖啡。
Then
系统退回所有硬币。
And
系统提示当前无法给出咖啡。
And
我无法保持清醒。

AC4:
Given
我是一名ThoughtWorker。
And
我持有低于一杯咖啡价格的硬币。
When
我给出硬币点一杯咖啡。
Then
系统退回所有硬币。
And
系统提示硬币不足。
And
我无法保持清醒。

AC5:
Give
我是一名ThoughtWorker。
And
我有一杯咖啡。
And
咖啡对我有效。
When
我喝下咖啡。
Then
我可以保持清醒。

AC6:
Give
我是一名ThoughtWorker。
And
我有一杯咖啡。
And
咖啡对我无效。
When
我喝下咖啡。
Then
我无法保持清醒。
