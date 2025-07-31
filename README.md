## サンプルデータ

### 📚 Bookデータ

POST `/api/books`

<details>

<summary>Bookデータ(3件)</summary>

📘 Book1
```json
  {
    "isbn": "978-4-7741-8411-1",
    "title": "ドメイン駆動設計入門",
    "description": "DDDの基礎を学べる書籍です。",
    "author": "山田太郎",
    "publicationDate": "2024-05-01T00:00:00+09:00"
}
```
📘 Book2
```json
{
    "isbn": "978-4-7981-5112-0",
    "title": "現場で使えるPHP設計入門",
    "description": "PHPで設計を意識した開発を学ぶための本。",
    "author": "佐藤花子",
    "publicationDate": "2023-11-15T00:00:00+09:00"
}
```
📘 Book3
```json
{
    "isbn": "978-4-7981-5382-7",
    "title": "実践Symfony",
    "description": "Symfonyフレームワークの実践ガイド。",
    "author": "高橋一郎",
    "publicationDate": "2022-08-20T00:00:00+09:00"
}
```

</details>

### 📝 Reviewデータ

POST `/api/reviews`

<details>

<summary>Reviewデータ(各Bookに対して複数のレビュー)</summary>

📘 Book ID 1 (/api/books/1) に対するレビュー

```json
{
    "rating": 5,
    "body": "とても分かりやすい内容でDDDが理解できました！",
    "author": "読者A",
    "publicationDate": "2024-05-10T00:00:00+09:00",
    "book": "/api/books/1"
}
```
```json
{
    "rating": 5,
    "body": "とても分かりやすい内容でDDDが理解できました！",
    "author": "読者A",
    "publicationDate": "2024-05-10T00:00:00+09:00",
    "book": "/api/books/1"
}
```

📘 Book ID 2 (/api/books/2) に対するレビュー

```json
{
    "rating": 3,
    "body": "基礎的な内容が多く、中級者には物足りないかも。",
    "author": "読者C",
    "publicationDate": "2023-12-01T00:00:00+09:00",
    "book": "/api/books/2"
}
```
```json
{
    "rating": 4,
    "body": "実際のコード例が豊富で理解しやすかった。",
    "author": "読者D",
    "publicationDate": "2023-12-03T00:00:00+09:00",
    "book": "/api/books/2"
}
```

📘 Book ID 3 (/api/books/3) に対するレビュー

```json
{
    "rating": 5,
    "body": "Symfonyの設計思想がよくわかる良書。",
    "author": "読者E",
    "publicationDate": "2022-09-01T00:00:00+09:00",
    "book": "/api/books/3"
}
```
```json
{
    "rating": 4,
    "body": "実践的だけど初心者には少し難しいかも。",
    "author": "読者F",
    "publicationDate": "2022-09-05T00:00:00+09:00",
    "book": "/api/books/3"
}
```

```json
{
    "rating": 4,
    "body": "図での表現もいくつかありわかりやすかった。",
    "author": "読者C",
    "publicationDate": "2022-09-03T00:00:00+09:00",
    "book": "/api/books/3"
}
```

</details>

