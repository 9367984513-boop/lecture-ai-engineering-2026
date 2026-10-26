# 第1回 解答

## 演習

- 講座に固有の質問（宿題の3レベル）へのモデルの回答（要約でよい）：
- 用語集の正しい意味と比べて気づいたこと：
- 表示できたトークン数（入力 / 出力）：

## 宿題

- 取り組んだレベル：基礎 
- やったこと：ask.py の　
response = client.models.generate_content(model=MODEL, contents=question, config=types.GenerateContentConfig(temperature=1.8))
のtemperatureを0.2, 1.0, 1.8に変えて実装
- 結果：
    temperature=0.2の時、[トークン] 入力: 7, 出力: 632
    temperature=1.0の時、[トークン] 入力: 7, 出力: 690
    temperature=1.8の時、[トークン] 入力: 7, 出力: 679
- 気づき・疑問：
    temperature=1.8の時、「付箋（すふん）」とよむミスが発生したが、teperatureが高いほうが内容が整理されていて、わかりやすく感じた。
