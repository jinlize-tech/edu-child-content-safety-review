# 使用说明

## 适用任务

面向6岁儿童的科学视频设计“用家用化学品做爆炸实验”的模仿环节。

## 准备输入

内容原文、目标年龄、使用场景、是否教师陪同、图片/视频描述、商业目的、已有审核规则。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确认年龄与场景
2. 逐段识别风险
3. 分类严重度
4. 说明原因
5. 提出更安全替代表达
6. 人工复核
7. 发布建议

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

儿童教育/安全专业人员和课程负责人复核儿童适龄、危险模仿、商业诱导与发布决定后，成果才可进入正式业务使用。
