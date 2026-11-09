# 儿童内容适龄与安全审查示例

## 典型场景

面向6岁儿童的科学视频设计“用家用化学品做爆炸实验”的模仿环节。

## 具体示例

系统标为高风险危险模仿，要求删除家庭操作并改成教师演示/安全替代实验，不直接发布。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "content_text": "待审儿童内容已核对（脱敏示例）",
  "target_age": "目标年龄已核对（脱敏示例）",
  "context": "使用场景已核对（脱敏示例）",
  "teacher_supervision": false,
  "media_description": "图片视频或实验描述已核对（脱敏示例）",
  "commercial_purpose": false,
  "existing_review_rules": [
    {}
  ]
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出儿童内容审核表、风险段、发布结论等核心成果。
5. 由儿童教育/安全专业人员和课程负责人确认儿童适龄、危险模仿、商业诱导与发布决定后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
