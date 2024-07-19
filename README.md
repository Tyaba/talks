# Talks
slidevのスライド置き場
# Links
- 参考にしたリポジトリ [antfu/talks](https://github.com/antfu/talks)
# 新規スライド作成手順
```bash
mkdir slide1
cd slide1
pnpm create slidev@latest  # project_name == src
$editor slide1/src/package.json
```
編集内容は下記
```slide1/src/package.json
{
 "name": "slidev",
 "type": "module",
 "private": true,
 "scripts": {
    + "build": "slidev build --base /slide1/ --out ../../dist/slide1",
    + "export": "slidev export --dark --output ../slide1.pdf"
 }
}
```