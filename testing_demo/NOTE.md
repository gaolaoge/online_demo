1. 为什么要做单元测试
2. 前端 Jest 单元测试实战
3. 前端组件化 UI 测试实战
4. 前端状态管理数据流测试
5. 前端单元测试该如何落地

> 写不好单元测试是能力问题，不写单元测试是态度问题

瀑布流开发：一轮「需求-设计-开发-测试-发布」，风险随开发进度不断升高，可能在测试阶段发现结果与需求并不完全匹配，最后推倒重做；
敏捷迭代开发：将需求分割，通过数轮「需求-设计-开发-测试-发布」迭代，最终达成目标，简单的说就是「迭代式」软件开发流程，每一轮迭代都可能会引入新的问题，但每一轮的风险都是相等的；

有1个关键指标来度量什么叫更快，也就是 Lead Time，它是指新产品推向市场的一个时间周期：一个 idea 从提出到被验证，再到最终生产，发布到线上环境面对用户的时间。

敏捷开发最重要的就是要「快」，快速迭代，持续交付用户价值。

敏捷开发对于开发者来说，没有「单元测试」，就快不起来：

1. 每次开发迭代，团队都需要投入人力来手工测试，这就导致了「人效」的问题；
2. 且没有单元测试，开发者往往倾向于不敢随意重构，导致代码逐渐腐化；
3. 随着项目进展，脚本越发复杂，导致开发速度再次降低，从而陷入死循环；

> 单元测试的存在与否应该是理性判断的，而不是出于个人的感性选择，
> 如果业务不需要频繁上线，并且整个团队有足够多的人力来覆盖手工测试，那就可以不写单元测试，
> 反之如果想随时重构脚本，就需要单元测试来进行自动还回归，保障功能不被破坏。

另外，开发者也会在项目中搭建流水线持续集成产品脚本和测试脚本，持续不断的验证每次的提交是否符合预期，
拥有这样的自动化套件可以帮助开发者快速验证提交的完整性。

前端测试分类：

1. e2e
2. 集成测试
3. 单元测试

单元测试：1. 写起来最快，2. 运行速度最快， 3. 反馈效果最直接；