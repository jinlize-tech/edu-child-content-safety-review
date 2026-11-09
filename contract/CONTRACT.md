# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `content_text` | 待审儿童内容 | string | 是 |
| `target_age` | 目标年龄 | string | 是 |
| `context` | 使用场景 | string | 是 |
| `teacher_supervision` | 是否教师陪同 | boolean | 是 |
| `media_description` | 图片视频或实验描述 | string | 否 |
| `commercial_purpose` | 商业目的 | boolean | 是 |
| `existing_review_rules` | 现有审核规则 | array | 否 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `儿童内容审核表`：结构化条目数组，不允许空壳或占位文本。
- `风险段`：结构化条目数组，不允许空壳或占位文本。
- `年龄适配建议`：结构化条目数组，不允许空壳或占位文本。
- `替换示例`：结构化条目数组，不允许空壳或占位文本。
- `需专业复核项`：结构化条目数组，不允许空壳或占位文本。
- `发布结论`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
