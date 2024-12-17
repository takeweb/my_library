# my_library"
# 『バックエンドエンジニアを目指す人のためのRust』 第7章 自作ライブラリを公開できるようになろう[本棚ツール]

## 環境構築
```
cargo new --lib my_library
```

## module構成
```
crate
└── library
    ├── bookモジュール
    │   └── Book構造体
    └── bookshelfモジュール
        └── Bookshelf構造体
```

## ファイルを分割
```
mkdir src/library
touch src/library/mod.rs
touch src/library/book.rs
touch src/library/bookshelf.rs
```

## GitHubに公開
```
echo "# my_library" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/takeweb/my_library.git
git push -u origin main
```