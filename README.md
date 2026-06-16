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
python sortrenamemovepdf.py -i ./inbox -o ./sorted
```
