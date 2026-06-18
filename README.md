# PDF 智能分类整理工具

扫描目录中的 PDF，提取内容并自动重命名、分类归档。

## 环境变量

复制 `.env.example` 为 `.env` 并填写：

- `OPENAI_API_KEY`：OpenAI 接口密钥

## 启动

```bash
pip install -r requirements.txt
python sortrenamemovepdf.py --help
```

## 示例

```bash
python sortrenamemovepdf.py -i ./inbox -c ./corrupted -r ./sorted

# 预览模式 / 限制解析页数
python sortrenamemovepdf.py -i ./inbox -c ./corrupted -r ./sorted --dry-run --max-pages 20
```

## 注意

- 启动前会校验输入/输出目录是否存在
- `--dry-run` 仅预览重命名，不移动文件
- `--max-pages` 控制送入 AI 的 PDF 页数上限
- 大批量处理前请备份原文件
