# 修復 macOS 之 Markdown 搜尋索引

Spotlight 對 Markdown 內容之索引時常出現錯誤，透過下列命令修復之：

```bash
git clone https://github.com/yuripe-murmur/Markdown.mdimporter.git
sudo cp -R Markdown.mdimporter /Library/Spotlight
mdimport -r /Library/Spotlight/Markdown.mdimporter
sudo mdutil -E /
``` 
