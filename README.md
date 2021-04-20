# README

## セットアップ

サイト作成

```shell
hugo new site hugo-meghna
```

レポジトリ初期化

```shell
cd hugo-meghna
git init
echo '*~' >> .gitignore
echo '*.bak' >> .gitignore
echo '*.orig' >> .gitignore
echo '.env' >> .gitignore
echo 'public' >> .gitignore
echo 'resources' >> .gitignore
```

テーマ設定(submoduleはhttpsプロトコルで追加)

```shell
git submodule add https://github.com/themefisher/meghna-hugo.git themes/meghna
```

(参考)submoduleの削除

```shell
git submodule deinit -f themes/meghna
git rm themes/meghna
rm -fr .git/modules/meghna
```

サイト設定

```shell
cp -p themes/meghna/exampleSite/config.toml .
cp -pr themes/meghna/exampleSite/{content,data} .
```

## Link

* [Meghna Hugo \| Hugo Themes](https://themes.gohugo.io/meghna-hugo/)
