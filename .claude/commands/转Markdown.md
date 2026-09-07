description: "调用 markitdown 将 PDF/Word/PPT/Excel 等文档转换为 Markdown 文本，便于在 Obsidian 中全文检索、引用与做阅读笔记"
steps:
  - "确定目标文件：从用户消息（可用 @ 语法或直接给路径）或当前笔记/上下文中识别要转换的文档（.pdf / .docx / .pptx / .xlsx / .html 等）"
  - "确认输出位置：默认在源文件同目录生成同名 .md；若用户指定路径则按指定路径"
  - "执行转换（路径用双引号包裹以防空格/撇号，如 Bruce's Vault）：
     markitdown \"<输入文件>\" -o \"<输出文件>.md\""
  - "核对结果：确认 .md 已生成且非空；抽查原文关键片段（音符、希腊字母、长音符号等非 ASCII 字符）是否保留"
  - "（可选）若用户要求，读入转换结果做结构化整理（补 frontmatter、wikilink、章节标题）"
