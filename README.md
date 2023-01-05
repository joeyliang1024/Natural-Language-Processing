# 自然語言處理
- [markdown語法教學](https://tiida54.github.io/2018/01/03/3%E5%88%86%E9%90%98%E5%AD%B8%E6%9C%83Markdown%E5%B8%B8%E7%94%A8%E8%AA%9E%E6%B3%95/)
## Homework1
- 命名實體辨別（Name Entity Recognition）
- 任務目標：識別出句子中的專有名稱。
- 總共22種類別。
- 使用 LSTM 和 GloVe 的 word embedding 進行訓練。
## Homework2
- 問答系統 (Question Answering)
- 任務目標：給定一篇文章和問題，找出文章中的正確答案。
- 屬於 ODQA(Open Domain Question Answering)。
- 必須使用TF-IDF 和 BM25 進行文章提取。
## Final_Project
- 比較ODQA的 generative 和 extractive 的結果表現。
- 參考論文：[A Copy-Augmented Generative Model for Open-Domain Question Answering](https://aclanthology.org/2022.acl-short.47.pdf)
  - Author: Shuang Liu, Dong Wang, Xiaoguang Li, Minghui Huang, Meizhen Ding
  - Publish: ACL 2022
  - add pointer network to fuss-in-decoder model
- generative model:FiD-PGN, bert2BERT
- extractive model: bert-base-uncased, 使用 TF-IDF 和 BM25 進行文章提取。
-<table>
    <tr>
        <th>score</th><th columnspan="5">TF-IDF</th><th>bert2BERT</th><th>FiD-PGN</th>
    </tr>
    <tr>
        <td>k</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>5</td><td>25</td>
    </tr>
    <tr>
        <td>LCS</td><td>123</td><td>123</td><td>123</td><td>123</td><td>123</td><td>123</td><td>123</td>
    </tr>
    <tr>
        <td>F1</td><td>92</td><td>92</td><td>92</td><td>92</td><td>92</td><td>92</td><td>92</td>
    </tr>
</table>
## AI CUP
## AI CUP
- [自然語言理解的解釋性資訊標記競賽](https://tbrain.trendmicro.com.tw/Competitions/Details/26)
- 機器學習模型的可解釋性（explainability）是人工智慧技術在落實與應用時，備受期待的項目。如果模型能夠在精準預測之餘，同時提供佐證其預測行為之依據，人類將有機會事先發現模型判斷的錯誤，大幅提高人類對模型之信賴，使得人工智慧技術更能落實到關鍵性的決策場域。
議論探勘（argument mining）是近期廣受矚目的自然語言處理任務。該任務試圖從文句中找出人們的主張（claim），以及支持或反對這些主張的原因。這可視為輿論探勘（opinion mining）或情緒分析（sentiment analysis）的進階任務。基礎的議論探勘任務，是給定一個主張（claim）與一個前提（premise），由模型判斷兩者之間的議論關係，例如該項前提為支持或反駁該主張。換言之，這是一個典型的分類任務，判斷一組主張與前提的關係。對於這類的任務，目前的自然語言處理模型已能達到一定的效能，近期的深度學習技術也顯示模型已能掌握部份議論推理能力。然而，模型在提供分類預測之餘，究竟是如何得到該預測之結果，其中的解釋性要素則仍然未有充份的研究。
有鑑於此，本計畫以議論探勘為目標，希望能讓模型在預測文句之間支持或反駁的關係之外，找出文句之中關鍵性的片段，作為預測的佐證資訊。這類資訊可以讓研究人員更了解模型內部的行為、促進自然語言處理的研究，同時也可望將來在終端應用時，提供出模型的判斷依據，讓人類評估模型該次判斷的可靠程度。
