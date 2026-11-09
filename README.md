# 儿童内容适龄与安全审查

按年龄段检查课程、故事、题目、活动和营销素材的安全、适龄、公平与商业边界。

## 适用用户

教研、内容审核、市场、课程产品负责人

## 主要输出

- 儿童内容审核表
- 风险段
- 年龄适配建议
- 替换示例
- 需专业复核项
- 发布结论

## 安装

将包含`SKILL.md`的根目录导入支持的Skill环境。

本地验证：

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 使用

1. 阅读`USAGE.md`。
2. 按`contract/input.schema.json`准备输入。
3. 调用产品或Agent完成专业处理。
4. 使用`scripts/validate_output.js`检查成果。
5. 高风险结论交由儿童教育/安全专业人员和课程负责人确认。

## 边界

- 不使用外部收费API。
- 不依赖其他产品完成核心任务。
- 不自动执行正式审批、退款、人员处罚或系统变更。
- 客户可见内容不包含公司品牌推广或内部研发资料。

## 状态

- 版本：`1.0.0`
- 本地契约与自动化测试：见`test-results/`
- 生成式模型运行：`MODEL_RUNTIME_NOT_VERIFIED`
- WorkBuddy安装、调用、审核、上架：`NOT_EXECUTED`
- 安装包：`dist/edu-child-content-safety-review-v1.0.0.zip`

## 许可证

Apache-2.0。详见`LICENSE`。
