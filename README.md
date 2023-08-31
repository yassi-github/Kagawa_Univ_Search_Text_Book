# Kagawa_Univ_Search_Text_Book

## 処理手順

1. 香川大学のドリームキャンパスから受講している講義の一覧を取得する
1. 受講している講義の教科書をシラバスから取得する
1. 結果をエクセルにまとめる

## build

```sh
docker compose up --build
```

## run python

```sh
docker exec kagawa_univ_search_text_book-app-1 python Search_Text_Book.py
```

## view browser

- use novnc

    access to `http://$(ip r get 1 | head -1 | cut -d' ' -f3):7900/` with your browser.
