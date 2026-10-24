# 初中数学改卷 Skill

免费分享的 Codex 技能包：逐题批改扫描答题卡，在原卷上标出扣分点，将疑点集中交给老师面批，最后输出批改试卷 ZIP 和班级成绩表。

## 下载与安装

- **[下载最新版技能包](https://github.com/wwwxxxttthhh/math-exam-grading/releases/latest/download/math-exam-grading.zip)**
- [查看版本说明和历史版本](https://github.com/wwwxxxttthhh/math-exam-grading/releases)

下载后，将 ZIP 放入自己的工作文件夹，在 Codex 中引用文件并发送：

> 请将这个压缩包里的 math-exam-grading 安装到本机可识别的个人技能目录，保留 references、scripts 和 agents；若已有同名技能，先备份。检查引用文件和所需文档处理工具是否齐全，并确认可以调用。

ZIP 内另附完整安装使用说明。不要直接照抄他人电脑的绝对路径。

## 适用范围与使用条件

- 当前只适用于初中数学。
- 需要能够处理本地文件的 Codex 及相应文档、表格、图像工具。此包是技能指令和辅助脚本，不是独立桌面软件。
- 技能包免费；模型、平台或其他工具是否收费取决于使用环境。
- 离线功能指教师面批 HTML；AI 批改本身仍需要相应运行环境。
- 教师负责核对评分细则、复核疑点和确认最终成绩，建议先用少量试卷试跑。

## 准备四种材料

1. 原试卷。
2. 参考答案和评分细则。
3. 空白答题卡。
4. 按班级标明的学生扫描 ZIP。

## 主要功能

- 逐题阅读作答，记录小问得分和具体扣分依据，认可正确的等价方法。
- 在原得分栏打勾，解答题用红色细圈、框线或箭头标出扣分处，在空白处简注原因。
- 需要复核时生成图片内嵌、可离线打开的面批 HTML；按题号和小问集中排列，同题连续复核。
- 教师提交面批结果后，同步成绩、勾分位置和红笔批注。
- 最终默认只交付批改 ZIP 与班级成绩 XLSX，多班在工作簿中分表。
- 保留原扫描格式、文件名、顺序及目录结构；具体扫描系统兼容性需实际试扫。

## 调用示例

```text
请使用 $math-exam-grading 批改本次初中数学试卷。
材料包括原试卷、参考答案和评分细则、空白答题卡、按班级区分的扫描 ZIP。
解答题在原卷红笔圈出扣分点并简注原因；疑点提供同题集中排列、图片内嵌的离线面批 HTML。
最终只交付批改试卷 ZIP 和班级成绩 XLSX。
```

## 包内内容

```text
math-exam-grading/
  SKILL.md
  agents/openai.yaml
  references/grading-record.md
  references/interactive-review.md
  references/class-review-lessons.md
  scripts/repack_scans.py
安装使用说明.txt
```

不包含学生姓名、成绩、扫描件或考试答案。反馈问题时请勿上传可识别学生身份的资料。

官方技能说明：[Build skills](https://learn.chatgpt.com/docs/build-skills)。