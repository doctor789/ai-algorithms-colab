# AIのアルゴリズムと原理 — 実習ノートブック(全15回)

「AIのアルゴリズムと原理」の講義動画に対応した、Python 実習ノートブックです。
**インストール不要**。下のリンクをクリックすれば、ブラウザ(Google Colab)でそのまま動きます。

📺 **講義動画の再生リスト:** https://www.youtube.com/playlist?list=PLXcfgShBCvSc

---

## この授業の特徴

**スライドに出てくる数字は、すべて実際に測ったものです。** 教科書から引用した値は1つもありません。
そして、**予想が外れた回もそのまま載せています**(第8回・第10回・第12回・第14回)。

ノートブックを動かすと、講義と同じ数字が手元で再現できます。
数字が少し違うこともあります(モデルを学習しなおす回など)。そのときは、なぜ違うのかを考えてみてください。

---

## 使い方

1. 下の表から、その回の「開く」をクリック
2. 上から順にセルを実行(セルを選んで **Shift + Enter**)
3. 最初のセルで日本語フォントなどを入れるので、1〜2分かかります
4. コードは自由に書き換えて構いません。**壊しても大丈夫**です(開き直せば元に戻ります)

保存したいときは、Colab のメニューから「ドライブにコピーを保存」を選んでください。

> **時間のかかる回があります**
> 第10回(モデルを数GBダウンロード)、第12回(拡散モデルを一から学習・10分ほど)、
> 第13回(3GBのモデル)は、実行を始めてから説明を読むのがおすすめです。

---

## 各回のノートブック

**各回は独立しています。** どの回から始めても、そこだけで完結します。

| 回 | 内容 | 実習でやること | 動画 | ノートブック |
|---|---|---|---|---|
| 1 | いまのAIは何ができて、何ができないか | strawberry の分割を見て、次の語の確率と温度を動かす | [▶](https://youtu.be/Kq_AmBskk38) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A01_intro.ipynb) |
| 2 | 機械学習とは | 丸暗記モデルを作り、訓練誤差ほぼ0でも役に立たないことを確かめる | [▶](https://youtu.be/UZfnYTanBCQ) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A02_ml_basics.ipynb) |
| 3 | 分類の評価 | しきい値を動かし、見逃しと空振りが入れ替わるのを見る | [▶](https://youtu.be/zmte62pNz8U) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A03_evaluation.ipynb) |
| 4 | ニューラルネットワーク | XOR を1層で解かせて失敗させ、2層にして解く。ReLU を外すと戻る | [▶](https://youtu.be/mDY-4FA7_dk) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A04_neural_net.ipynb) |
| 5 | 学習のしくみ | 勾配降下法で谷を下り、発散を目撃する。過学習を再現して対策を測る | [▶](https://youtu.be/QtEN0VBon9Y) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A05_training.ipynb) |
| 6 | 画像認識 | フィルタを手書き数字に当てる。CNN と MLP を比べ、ずらしへの強さを測る | [▶](https://youtu.be/X4OOk5V_A2s) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A06_cnn.ipynb) |
| 7 | 埋め込み | 文を384個の数にして近さを測る。否定が見分けられないことを確かめる | [▶](https://youtu.be/LsGKglcTJxA) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A07_embedding.ipynb) |
| 8 | Transformer | 144個の注意ヘッドをのぞく。教科書の有名な図の再現を自分で試す | [▶](https://youtu.be/jDI0y79v3nY) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A08_transformer.ipynb) |
| 9 | 強化学習 | スロットで探索と活用を比べ、報酬設計を3通り壊してみる | [▶](https://youtu.be/Uf8zNy8KfMQ) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A09_rl.ipynb) |
| 10 | 大規模言語モデル | 3サイズの loss を測ってスケーリング則を見る。「創発」を2つの指標で測る | [▶](https://youtu.be/y2KeVGuf-Dw) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A10_llm.ipynb) |
| 11 | プロンプトとRAG | 書き方で答えがどう変わるかを測る。RAG を自分で組んで、限界を見る | [▶](https://youtu.be/8HRDX_kGpSM) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A11_rag.ipynb) |
| 12 | 画像生成 | 拡散モデルを一から学習させ、生成物が訓練画像の写しかを測る | [▶](https://youtu.be/7sQrmV4V4NY) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A12_diffusion.ipynb) |
| 13 | なぜ間違えるのか | 存在しない国の首都を聞く。何度も聞いて「知らない」を見抜く | [▶](https://youtu.be/iIMMGLcQMJk) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A13_hallucination.ipynb) |
| 14 | 説明可能性と社会 | 木と森を比べ、3つの重要度を出し、公平さを測って揃えてみる | [▶](https://youtu.be/oLtnj8E9n0c) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A14_fairness.ipynb) |
| 15 | 総まとめ | 「正解率84.6%」を5つの視点で分解する | [▶](https://youtu.be/Cm4WeLIf0iE) | [開く](https://colab.research.google.com/github/doctor789/ai-algorithms-colab/blob/main/notebooks/A15_summary.ipynb) |

---

## この授業の考え方

AI は毎年入れ替わります。今日いちばん良いモデルは、数年後には誰も使っていません。
だからこの授業では、**個々の技術ではなく「測りかた」**のほうを扱います。

全15回のスライドに **「今日わかったこと・まだ言えないこと」** の枠を必ず置いてあります。
ノートブックでも、動かして終わりではなく、**限界を確かめるセル**を入れてあります。

くり返し出てくる形:

1. **1つの数字では性能を表せない** — 84.6% は5つの数字に分かれる(第3・15回)
2. **訓練で良くても本番で良いとは限らない** — 検証誤差は40回目で底を打つ(第2・5回)
3. **見せていないものには弱い** — 4画素ずらすと 95.1% → 45.1%(第6回)
4. **指標を最適化すると、指標だけが上がる** — 報酬5倍でも仕事はしていない(第9回)
5. **比べる相手がなければ、数字に意味はない** — 「85%似ている」は証拠にならない(第12回)
6. **公平の定義は複数あり、両立しない** — 揃えると偏りが場所を変える(第14回)

### 講義で渡す「14の質問」

技術の名前は忘れても、これだけは残してほしい、というものです。

| # | 質問 | 出どころ |
|---|---|---|
| 1 | もっともらしさで足りる仕事か、正確さが要る仕事か | 第1回 |
| 2 | その精度は、学習に使っていないデータでの数字か | 第2回 |
| 3 | 見逃しと空振り、それぞれ何件か | 第3回 |
| 4 | その改善は、非線形を足したからか | 第4回 |
| 5 | 訓練誤差だけでなく、検証誤差はどうだったか | 第5回 |
| 6 | それは、どういう変化まで耐えられるか | 第6回 |
| 7 | 意味を理解しているのか、似た文脈を測っているのか | 第7回 |
| 8 | その図は、どのモデルの、どの層の、どのヘッドか | 第8回 |
| 9 | その数字が上がったとき、実際の振る舞いはどうだったか | 第9回 |
| 10 | その改善は、私の用途でも改善か | 第10回 |
| 11 | その出典、実際に開いて読んだか | 第11回 |
| 12 | その数字は、何と比べた数字か | 第12回 |
| 13 | それ、言い方を変えて3回聞いたか | 第13回 |
| 14 | その説明は誰に向けたものか / どの公平を選び、何を諦めたか | 第14回 |

> ただし、**14個すべてをいつでも使うわけではありません。**
> どれが当てはまるかを選べること自体が、技術を理解しているということです(第15回・演習3)。

---

## 必要なもの

Google アカウントだけです。Python のインストールは不要です。

自分のパソコンで動かす場合は、回によって次が必要です。

- 全回共通:`numpy` `matplotlib` `japanize-matplotlib`
- 第2・3・14・15回:`scikit-learn`
- 第4・5・6・12回:`torch`(第6・12回は `torchvision` も)
- 第1・8・10・13回:`transformers`
- 第7・11回:`sentence-transformers`

## ライセンス

MIT License。授業・自習・改変、自由にお使いください。
