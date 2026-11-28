# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前：glossary_search_glossary
- STEP 2 の [tool call]：glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]：fetch_fetch({'url': 'https://modelcontextprotocol.io/'})
- STEP 4 の [tool call]：aws_aws___search_documentation({'search_phrase': 'Amazon S3 versioning overview', 'topics': ['general']})
- 気づき・疑問：MCPサーバが簡単に使える。ただし、外部のMCPサーバはブラックボックス。閉じた環境では、UVXも使えないと思った。

## 宿題

<!-- 基礎・実装・発展のどれか1つに取り組めば完了です。 -->

- 取り組んだレベル：基礎
- やったこと：mcp_server.pyに [glossary_get_lecture_summary]を追加したのみ。mcp_agent.pyは修正していない。その後第2回の講義内容を確認
- 結果：[tool call]   glossary_get_lecture_summary({'lecture': 2})　[tool return] glossary_get_lecture_summary -> # 第2回 ファインチューニングとLoRA
- 気づき・疑問：agentを修正することなく、MCPサーバに追加するだけで、機能が使えることが分かった。　疑問としては、追加できる最大数などあるのか。
