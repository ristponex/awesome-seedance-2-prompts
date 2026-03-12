<!--
  Awesome Seedance 2.0 プロンプト集
  日本語版
-->

<div align="center">

```
   ___                                           ___                    __                           ___      ___
  / __| ___  ___  __| | __ _  _ _   __  ___     |_  )       _ __  _ _ / _ \ _ __   _ __  | |_  ___  |_  )    / _ \
  \__ \/ -_)/ -_)/ _` |/ _` || ' \ / _|/ -_)     / /    _  | '_ \| '_| (_) | '  \ | '_ \ | __|(_-<   / / _  | (_) |
  |___/\___|\___|\__,_|\__,_||_||_|\__|\___|    /___|   (_) | .__/|_|  \___/|_|_|_|| .__/ |_|  /__/  /___(_)  \___/
                                                            |_|                    |_|
```

# Awesome Seedance 2.0 プロンプト集

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/atlascloud/awesome-seedance-2-prompts?style=social)](https://github.com/atlascloud/awesome-seedance-2-prompts/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Last Commit](https://img.shields.io/github/last-commit/atlascloud/awesome-seedance-2-prompts)](https://github.com/atlascloud/awesome-seedance-2-prompts/commits/main)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/atlascloud/awesome-seedance-2-prompts/pulls)
[![Seedance](https://img.shields.io/badge/Seedance-2.0-blue?logo=bytedance&logoColor=white)](https://seed.bytedance.com/)
[![Atlas Cloud](https://img.shields.io/badge/今すぐ試す-Atlas%20Cloud-orange)](https://www.atlascloud.ai?ref=JPM683)

**ByteDance の Seedance 2.0 のための高品質プロンプト、テクニック、リソースの厳選コレクション — 世界最先端の統合マルチモーダル AI 動画生成モデル。**

CNN はこれを **「ハリウッドを震撼させるほど強力な中国の最新 AI」** と評しました。

[English](README.md) | [中文](README_zh-CN.md) | [日本語](README_ja.md) | [한국어](README_ko.md)

---

**役に立ったら、このリポジトリにスターをお願いします！** 皆様のサポートがより多くのクリエイターにこのリソースを届けます。

</div>

---

<div align="center">

### Atlas Cloud でこれらのプロンプトを即座に実行

Seedance 2.0 を最高品質で体験する最速・最安の方法。

**無検閲 AI** | **最安値 $0.222/動画** | **2倍速の推論**

[![Atlas Cloud を試す](https://img.shields.io/badge/Atlas%20Cloud%20を試す-無料で開始-ff6b35?style=for-the-badge&logo=rocket&logoColor=white)](https://www.atlascloud.ai?ref=JPM683)

新規ユーザーは初回チャージで **25% ボーナス** 獲得（最大 $100）

</div>

---

## 目次

- [Seedance 2.0 について](#seedance-20-について)
- [クイックスタート（API）](#クイックスタートapi)
- [プロンプト集](#プロンプト集)
  - [超リアルな動画生成](#1-超リアルな動画生成)
  - [キャラクター＆シーンの一貫性](#2-キャラクターシーンの一貫性)
  - [高度なカメラワーク](#3-高度なカメラワーク)
  - [クリエイティブ視覚効果](#4-クリエイティブ視覚効果)
  - [ストーリー展開＆拡張](#5-ストーリー展開拡張)
  - [音声＆ボイス合成](#6-音声ボイス合成)
- [プロンプトエンジニアリングのコツ](#プロンプトエンジニアリングのコツ)
- [公式リソース](#公式リソース)
- [コミュニティリソース](#コミュニティリソース)
- [料金比較](#料金比較)
- [よくある質問](#よくある質問)
- [スター履歴](#スター履歴)
- [コントリビュート](#コントリビュート)
- [ライセンス](#ライセンス)

---

## Seedance 2.0 について

**Seedance 2.0** は ByteDance が **2026年2月** にリリースした次世代 AI 動画生成モデルです。**統合マルチモーダル音声視覚同時生成** を単一アーキテクチャで実現した初の実用モデルであり、一つのプロンプトから映画品質の動画、同期音声、セリフ、音楽、マルチショットの物語を生成します。

### コア機能

| 機能 | 詳細 |
|:-----|:-----|
| **統合音声視覚生成** | 単一モデルが動画＋同期音声＋セリフを一度に生成 |
| **複雑なカメラワーク** | プッシュプルズーム、フォーカス切替、トラッキングショット、POV切替、ヒッチコックズームなど |
| **マルチショット物語** | キャラクターとシーンの一貫性を保った連続マルチショットシーケンスの生成 |
| **8言語以上のリップシンク** | 日本語、英語、中国語、韓国語など8言語以上の音素レベルリップシンク |
| **キャラクター一貫性** | 画像/動画参照（`@image1`、`@video1`）によるショット間のキャラクター一貫性維持 |
| **シネマティック品質** | ハリウッド級のビジュアル品質、リアルなライティング、被写界深度、モーションブラー |

### 主要スペック

| スペック | 値 |
|:---------|:---|
| 最大解像度 | 最大 1080p |
| 動画長さ | 生成ごとに 5秒〜20秒 |
| アスペクト比 | 16:9、9:16、1:1、4:3、3:4 |
| オーディオ | ステレオ |
| フレームレート | 24fps / 30fps |
| 入力モード | テキスト→動画、画像→動画、動画→動画 |
| 参照サポート | 複数画像（`@image1`、`@image2`）、動画参照（`@video1`） |

### 活用シーン

- **映画制作＆プリビズ** — ストーリーボードから動画への迅速変換、コンセプト可視化、VFXプレビュー
- **広告＆マーケティング** — 商品CM、ブランドキャンペーン、SNS広告
- **SNS＆UGC** — ショート動画コンテンツ、TikTok/Reels、クリエイティブストーリーテリング
- **EC** — 商品紹介動画、バーチャル試着、ライフスタイルデモ
- **教育＆トレーニング** — 解説動画、歴史再現、科学の可視化
- **音楽＆エンタメ** — MV、歌詞動画、コンサート映像

---

## クイックスタート（API）

Atlas Cloud の API で Seedance 2.0 を数秒で実行。GPU設定は不要です。

### API キーの取得

1. [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683) でサインアップ
2. ダッシュボードの **API Keys** へ移動
3. 新しいキーを作成してコピー

### cURL の例

```bash
# Atlas Cloud API で Seedance 2.0 動画生成を呼び出す
curl -X POST "https://api.atlascloud.ai/api/v1/model/generateVideo" \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -d '{
    "model": "seedance-v1.5-pro",
    "input": {
      "prompt": "Fixed camera shot, a girl elegantly hanging clothes to dry, after finishing she takes out another piece from the basket and shakes the clothes vigorously. Sunlight filters through the fabric creating beautiful light rays. Cinematic lighting, 4K quality.",
      "negative_prompt": "blurry, low quality, distorted",
      "duration": 10,
      "aspect_ratio": "16:9"
    }
  }'
```

### Python の例

```python
import requests
import time

# Atlas Cloud API 設定
API_KEY = "YOUR_API_KEY"
BASE_URL = "https://api.atlascloud.ai/api/v1/model"

def generate_video(prompt: str, duration: int = 10, aspect_ratio: str = "16:9"):
    """
    Seedance 2.0 モデルで動画を生成する

    引数:
        prompt: 動画生成プロンプト
        duration: 動画の長さ（秒）
        aspect_ratio: 動画のアスペクト比
    戻り値:
        動画生成タスクの結果
    """
    # 動画生成リクエストを送信
    response = requests.post(
        f"{BASE_URL}/generateVideo",
        headers={
            "Content-Type": "application/json",
            "Authorization": f"Bearer {API_KEY}"
        },
        json={
            "model": "seedance-v1.5-pro",
            "input": {
                "prompt": prompt,
                "negative_prompt": "blurry, low quality, distorted",
                "duration": duration,
                "aspect_ratio": aspect_ratio
            }
        }
    )

    result = response.json()
    task_id = result.get("task_id")
    print(f"タスク送信完了、ID: {task_id}")

    # 生成状態をポーリングで確認
    while True:
        status_resp = requests.get(
            f"{BASE_URL}/task/{task_id}",
            headers={"Authorization": f"Bearer {API_KEY}"}
        )
        status = status_resp.json()

        if status["status"] == "completed":
            print("動画生成完了！")
            return status["output"]["video_url"]
        elif status["status"] == "failed":
            raise Exception(f"生成失敗: {status.get('error')}")

        time.sleep(5)  # 5秒ごとに状態を確認

# 使用例
video_url = generate_video(
    prompt="Camera slightly pulls back revealing the full street view and follows "
           "the female protagonist moving. The wind blows the hem of her dress as "
           "she walks on the streets of 19th century London. Cinematic lighting, "
           "film grain, anamorphic lens.",
    duration=15,
    aspect_ratio="16:9"
)
print(f"動画ダウンロードURL: {video_url}")
```

---

## プロンプト集

> **使い方**：以下のプロンプトをコピーして [Atlas Cloud プレイグラウンド](https://www.atlascloud.ai?ref=JPM683) に直接ペーストするか、API で使用してください。`@image1` や `@video1` を含むプロンプトは、参照画像/動画を先にアップロードしてください。

---

### 1. 超リアルな動画生成

フォトリアリスティックな動画出力のためのプロンプト。自然な動きとシネマティック品質を備えています。

| # | タイトル | 難易度 | 長さ | アスペクト比 |
|:--|:--------|:-------|:-----|:------------|
| 1.1 | エレガントな洗濯シーン | 初級 | 10秒 | 16:9 |
| 1.2 | 絵画の中のインタラクティブキャラクター | 中級 | 10秒 | 9:16 |
| 1.3 | ヴィクトリア朝の街並み | 中級 | 15秒 | 16:9 |
| 1.4 | 障害物チェイスシーン | 上級 | 15秒 | 16:9 |

<details>
<summary><b>1.1 エレガントな洗濯シーン</b> — 自然な物理表現の穏やかな日常</summary>

**プロンプト：**
```
Fixed camera shot, a girl elegantly hanging clothes to dry, after finishing she takes out
another piece from the basket and shakes the clothes vigorously. The fabric flows naturally
in the breeze. Sunlight filters through the wet fabric creating beautiful light diffusion.
Warm afternoon lighting, shallow depth of field, 4K cinematic quality.
```

**コツ：**
- 「Fixed camera」の指示でショットを安定させ、被写体の動きに焦点を当てる
- 「shakes the clothes vigorously」が Seedance 2.0 の物理シミュレーション能力をテスト
- 光の相互作用の詳細（「sunlight filters through」）を追加してリアリズムを向上

</details>

<details>
<summary><b>1.2 絵画の中のインタラクティブキャラクター</b> — 第四の壁を破る絵画アート</summary>

**プロンプト：**
```
The character in the painting has a guilty expression, eyes looking left and right, then
peeks out of the frame, quickly extends their hand out of the frame to grab a cola and
takes a sip. After drinking, they let out a satisfied sigh, wipe their mouth, and retreat
back into the painting, resuming their original elegant pose as if nothing happened.
Oil painting style blending with photorealistic elements. Warm gallery lighting.
```

**コツ：**
- このプロンプトは芸術スタイルとリアリズムを融合する Seedance 2.0 の能力を実証
- 連続アクション（覗く、掴む、飲む、戻る）が時間的一貫性をテスト
- SNS向けコンテンツに最適 — 共有性が高く魅力的

</details>

<details>
<summary><b>1.3 ヴィクトリア朝の街並み</b> — トラッキング付き時代劇シネマトグラフィー</summary>

**プロンプト：**
```
Camera slightly pulls back (revealing the full street view) and follows the female
protagonist moving. The wind blows the hem of her dress as she walks on the streets
of 19th century London. Gas lamps flicker along cobblestone streets. Horse-drawn
carriages pass in the background. Pedestrians in period-appropriate attire populate
the scene. Fog rolls gently through the narrow lanes. Cinematic color grading with
desaturated tones, film grain, anamorphic lens flare. 4K resolution.
```

**コツ：**
- カメラプルバック＋トラッキングでダイナミックでプロフェッショナルなカメラワークを実現
- 時代特有のディテール（ガス灯、石畳、馬車）がモデルを適切にガイド
- 「アナモルフィックレンズフレア」と「フィルムグレイン」でフィルム品質を追加

</details>

<details>
<summary><b>1.4 障害物チェイスシーン</b> — 複数キャラクターのハイペースアクション</summary>

**プロンプト：**
```
Camera follows a man in black clothes fleeing quickly through a crowded marketplace,
with a group of people chasing behind. He knocks over fruit stalls, ducks under hanging
fabrics, and leaps over a cart. The chasers stumble over the obstacles he leaves behind.
Handheld camera feel with slight shake. Fast-paced editing rhythm. Dramatic shadows and
high contrast lighting. Urban environment, daytime. Cinematic action movie style.
```

**コツ：**
- 複数キャラクターの相互作用がモデルの空間推論能力をテスト
- 環境の破壊（屋台を倒す）がダイナミックな複雑さを追加
- 「ハンドヘルドカメラ感」で本格的なアクション映画の美学を演出

</details>

---

### 2. キャラクター＆シーンの一貫性

参照画像・動画（`@image1`、`@video1`）を活用してキャラクターのアイデンティティとシーンの連続性を維持するプロンプト。

| # | タイトル | 参照タイプ | 難易度 | 長さ |
|:--|:--------|:----------|:-------|:-----|
| 2.1 | 退社後の帰宅 | `@image1` | 中級 | 10秒 |
| 2.2 | 歌舞伎舞台変換 | `@video1` | 上級 | 15秒 |
| 2.3 | ワンテイク・シームレス転場 | なし | 上級 | 20秒 |
| 2.4 | 高級ハンドバッグCM | `@image1` + `@image2` | 中級 | 10秒 |

<details>
<summary><b>2.1 退社後の帰宅</b> — 参照画像からの一貫性あるキャラクター</summary>

**プロンプト：**
```
@image1 The woman in the reference image arrives home after a long day at work. She opens
the front door, drops her bag on the hallway table, kicks off her heels, and walks to the
kitchen. She opens the refrigerator, the cool light illuminates her tired but content face.
She grabs a bottle of water and takes a long sip. Warm interior lighting transitioning to
cool refrigerator light. Cinematic, intimate atmosphere. 16:9 aspect ratio.
```

**コツ：**
- `@image1` がキャラクターの顔、髪型、体型を保持
- 連続シーン転場（廊下→キッチン→冷蔵庫）が空間一貫性をテスト
- シーン全体の照明変化が制作価値を向上

</details>

<details>
<summary><b>2.2 歌舞伎舞台変換</b> — 動画参照によるスタイル転換</summary>

**プロンプト：**
```
@video1 Transform this performance into a grand Chinese opera stage setting. The performer
maintains the same movements and expressions from the reference video, but is now wearing
elaborate Peking opera costume with ornate headdress. The stage features traditional red
and gold decorations, dramatic theatrical lighting with colored spotlights. Smoke effects
drift across the stage floor. Traditional Chinese instrumental accompaniment plays in sync
with the movements. Cinematic wide shot gradually pushing in to medium close-up.
```

**コツ：**
- `@video1` が参照動画からの動きとタイミングを保持
- モダンから伝統的な京劇へのスタイル変換がモデルの創造的範囲をテスト
- 音声生成が視覚的変換と同期するよう指定

</details>

<details>
<summary><b>2.3 ワンテイク・シームレス転場</b> — 複雑な長回しショット</summary>

**プロンプト：**
```
A continuous one-take shot: Starting in a busy modern office, the camera follows a young
woman as she walks toward the elevator. As the elevator doors open, the environment
seamlessly transforms into a lush tropical forest. She continues walking, now in explorer
attire, pushing through giant leaves. She parts a curtain of vines to reveal an ancient
temple. She steps inside and the interior transforms into a futuristic space station
control room. She sits down at the command console and the stars outside the window begin
to streak as the ship jumps to hyperspace. Smooth dolly movement throughout. No cuts.
Seamless environment transitions. Cinematic lighting adapts to each environment.
```

**コツ：**
- Seedance 2.0 の空間転場能力をテストする上級プロンプト
- 「No cuts」と「seamless」が連続性を保つための重要な指示
- 各環境にそれぞれ異なるライティングと雰囲気が必要
- 推奨時間：フル効果には20秒

</details>

<details>
<summary><b>2.4 高級ハンドバッグCM</b> — デュアル参照の商品フォーカス広告</summary>

**プロンプト：**
```
@image1 @image2 A luxury fashion commercial. The model from @image1 carries the handbag
from @image2. She walks confidently down a marble hallway in a grand European hotel.
Camera tracks alongside her at waist level, keeping the handbag in focus. She pauses at
a large window, golden hour light streams in, illuminating the bag's leather texture and
metallic hardware. She runs her fingers along the bag's stitching. Shallow depth of field,
the background softly blurs. Cut to a tabletop shot of the bag alone on a velvet surface
with dramatic side lighting. Premium commercial quality, 4K.
```

**コツ：**
- デュアル参照（`@image1` モデル用、`@image2` 商品用）で精密なブランド制御
- ウエストレベルのカメラで商品を常に目立たせる
- ゴールデンアワー＋浅い被写界深度はラグジュアリー商品撮影の成功法則

</details>

---

### 3. 高度なカメラワーク

Seedance 2.0 の業界最高水準のカメラ制御能力を披露するプロンプト。

| # | タイトル | カメラ技術 | 難易度 | 長さ |
|:--|:--------|:----------|:-------|:-----|
| 3.1 | エレベーターでのヒッチコックズーム | ドリーズーム（めまい効果） | 上級 | 10秒 |
| 3.2 | 複雑な廊下チェイス | トラッキング＋フォーカスプル | 上級 | 15秒 |
| 3.3 | 自動車CM シネマトグラフィー | オービタル＋クレーン＋トラッキング | エキスパート | 15秒 |
| 3.4 | 格闘技アクションシーン | ダイナミック多角度 | 上級 | 10秒 |

<details>
<summary><b>3.1 エレベーターでのヒッチコックズーム</b> — 古典的めまい/ドリーズーム効果</summary>

**プロンプト：**
```
A man stands alone in a modern glass elevator ascending a tall building. As the elevator
rises, execute a Hitchcock dolly zoom effect — the camera physically moves backward while
zooming in, making the background stretch and distort while the man's size stays constant.
His expression shifts from calm to uneasy as the effect intensifies. The city skyline
visible through the glass walls appears to warp and stretch. Dramatic orchestral tension
builds. Cool blue-gray color grading, sharp focus on subject, background distortion.
Vertigo-inspired cinematography.
```

</details>

<details>
<summary><b>3.2 複雑な廊下チェイス</b> — マルチテクニック・トラッキングショット</summary>

**プロンプト：**
```
A long dimly-lit hospital corridor. Camera starts with a close-up of running feet, then
rapidly tilts up to reveal a nurse sprinting down the hallway. Camera switches to tracking
alongside her, matching her pace. She bursts through double doors — camera momentarily
loses her behind the doors, then rack focuses to find her again at the end of the next
corridor. She slides around a corner, camera executes a whip pan to follow. Emergency red
lights begin flashing. The camera pulls back into a wide shot as she reaches the emergency
room doors. Urgent, tense atmosphere. Desaturated color palette with red accent lighting.
Handheld camera energy.
```

</details>

<details>
<summary><b>3.3 自動車CM シネマトグラフィー</b> — プレミアム自動車映像</summary>

**プロンプト：**
```
A sleek black sports car drives along a winding coastal highway at golden hour. Shot
sequence: (1) Orbital shot circling the car as it's parked on a cliff overlook, sunset
behind. (2) Low-angle tracking shot from road level as the car accelerates past, capturing
tire spin and road spray. (3) Crane shot starting from ground level, rising to aerial view
as the car navigates a serpentine curve. (4) Interior dashboard POV showing the road ahead
through the windshield, steering wheel turning. (5) Final aerial pullback revealing the
entire coastline with the car as a small moving element. Each shot transitions with smooth
motion blur cuts. Rich, warm color grading. Engine sound design included.
```

</details>

<details>
<summary><b>3.4 格闘技アクションシーン</b> — ダイナミック・アクション・シネマトグラフィー</summary>

**プロンプト：**
```
Two martial artists face off in a traditional wooden dojo. The first fighter launches a
spinning roundhouse kick — camera captures it in slight slow motion from a low angle.
The second fighter ducks and counters with a sweep kick, camera rapidly drops to ground
level to follow the leg motion. Quick cut to an over-the-shoulder POV as the first
fighter recovers and throws a combination of punches. Camera weaves between the fighters
like a third participant. Final move: the second fighter executes a flying knee — captured
in dramatic slow-motion with a 180-degree rotating camera angle. Impact moment freezes
for a beat. Wooden dust particles float in the air. Dramatic side lighting casting long
shadows. Sound of impacts and breathing.
```

</details>

---

### 4. クリエイティブ視覚効果

Seedance 2.0 の超現実的、芸術的、エフェクト豊富なコンテンツ生成能力を探るプロンプト。

| # | タイトル | スタイル | 難易度 | 長さ |
|:--|:--------|:--------|:-------|:-----|
| 4.1 | VRグラス宇宙旅行 | SF / 超現実 | 上級 | 15秒 |
| 4.2 | ファッション早着替えCM | ファッション / VFX | 中級 | 10秒 |
| 4.3 | 水墨画太極拳 | 伝統芸術 / モーション | 中級 | 15秒 |
| 4.4 | 魔法変身シーケンス | ファンタジー / VFX | 上級 | 10秒 |
| 4.5 | 金色パーティクルタイトル出し | モーショングラフィックス | 中級 | 8秒 |

<details>
<summary><b>4.1 VRグラス宇宙旅行</b> — 没入型SFビジュアライゼーション</summary>

**プロンプト：**
```
Close-up of a person putting on sleek VR glasses. As the glasses activate, the camera
pushes into the lens surface and transitions into a vast cosmic landscape. The viewer
flies through a nebula of swirling purple and blue gases, past glowing star clusters.
A massive planet rises into view, its rings catching starlight. The camera descends
through the planet's atmosphere into an alien cityscape with bioluminescent architecture.
Flying vehicles weave between organic towers. The journey reverses — pulling back through
space at increasing speed until we see the reflection of the cosmos in the VR lens, then
pull out to reveal the person removing the glasses with an expression of wonder. Seamless
macro-to-cosmic-to-macro transition. Epic orchestral soundtrack.
```

</details>

<details>
<summary><b>4.2 ファッション早着替えCM</b> — 高速衣装チェンジ</summary>

**プロンプト：**
```
A model stands in a pure white studio space, posing confidently. Every time she spins,
her outfit completely changes: Spin 1 — casual streetwear with sneakers. Spin 2 —
elegant black evening gown. Spin 3 — athletic wear mid-workout pose. Spin 4 — traditional
Japanese kimono. Spin 5 — futuristic metallic cyberpunk outfit. Each transition happens
mid-spin with a burst of fabric particles that dissolve and reform. Her hair and makeup
adapt to match each outfit. Camera circles her at a consistent distance. Upbeat pop music
rhythm syncs with each spin. Clean studio lighting with colored accent lights that change
to complement each outfit.
```

</details>

<details>
<summary><b>4.3 水墨画太極拳</b> — 中国伝統芸術のモーション表現</summary>

**プロンプト：**
```
A tai chi master performs fluid movements in a vast white void. His body and robes are
rendered in traditional Chinese ink wash painting style — black ink strokes forming his
silhouette, with varying ink density showing depth and shadow. As he moves, ink trails
flow from his hands and feet, painting landscapes in the air: mountains rise, rivers flow,
bamboo forests grow, cranes take flight. The ink spreads across the white space like water
on rice paper. His movements transition between tai chi forms — each form conjuring a
different natural element. The final movement brings all the ink paintings together into
a complete landscape scroll behind him. Traditional guqin music accompanies the movement.
Minimalist, meditative, artistic.
```

</details>

<details>
<summary><b>4.4 魔法変身シーケンス</b> — ファンタジー変身</summary>

**プロンプト：**
```
A young woman stands in an enchanted forest clearing at twilight. Fireflies surround her
as she raises her hands. Golden magical energy spirals up from the ground around her feet.
Her casual modern clothes begin to transform — fabric stretches and reshapes, colors shift
from denim blue to royal purple and gold. Armor-like shoulder pieces crystallize from
light particles. A flowing cape materializes behind her, catching an otherworldly wind.
Her hair lengthens and shifts color, adorned with glowing crystal accessories. A magical
staff materializes in her outstretched hand with a flash of light. She opens her eyes —
they now glow with golden light. She strikes a powerful pose as a shockwave of energy
ripples outward. Fantasy orchestral crescendo. Particle effects throughout. Cinematic
dramatic lighting.
```

</details>

<details>
<summary><b>4.5 金色パーティクルタイトル出し</b> — モーショングラフィックス・タイトルシーケンス</summary>

**プロンプト：**
```
Pure black background. A single golden spark appears in the center and begins to multiply
rapidly. Thousands of golden particles swirl in a controlled vortex, gradually forming
the letters of "SEEDANCE 2.0" in an elegant serif font. The particles settle into place
with micro-vibrations, each letter shimmering. Camera slowly pushes in. A wave of energy
passes through the text from left to right, causing each letter to briefly explode into
particles then reform with a more solid, metallic appearance. Subtle golden light rays
emanate from behind the text. A tagline fades in below: "Create the Impossible." Deep
cinematic bass impact sound on the title reveal, followed by an elegant tonal resolution.
Premium motion graphics quality.
```

</details>

---

### 5. ストーリー展開＆拡張

明確なストーリーアークを持つ物語主導の動画コンテンツ用プロンプト。

| # | タイトル | 物語タイプ | 難易度 | 長さ |
|:--|:--------|:----------|:-------|:-----|
| 5.1 | コミックパネルアニメーション | 連続物語 | 中級 | 15秒 |
| 5.2 | 幼少期の四季ドキュメンタリー | ドキュメンタリーモンタージュ | 上級 | 20秒 |
| 5.3 | コーヒーの朝キャンペーン | ブランドストーリー | 初級 | 10秒 |

<details>
<summary><b>5.1 コミックパネルアニメーション</b> — 静的パネルに命を吹き込む</summary>

**プロンプト：**
```
A comic book page with 4 panels is shown. Camera slowly zooms into the first panel — the
drawn world comes to life with subtle animation: a superhero stands on a rooftop, cape
fluttering. Panel border dissolves as the scene becomes full-frame. The hero leaps off
the building — mid-fall, the frame splits into the second panel showing the hero from a
different angle. Third panel: the hero lands in a dramatic three-point landing, cracks
spreading on the ground. Fourth panel: close-up of the hero standing up, eyes glowing,
with a speech bubble that reads "Time to save the city" — the text appears letter by
letter. Comic book color palette with bold outlines and halftone dot shading throughout.
Action sound effects appear as visual onomatopoeia ("WHOOSH", "CRACK"). Dynamic comic
book soundtrack.
```

</details>

<details>
<summary><b>5.2 幼少期の四季ドキュメンタリー</b> — 感動的なタイムラプス物語</summary>

**プロンプト：**
```
A documentary-style montage of a child growing through the seasons in a small rural
village. Spring: a toddler (age 3) takes first steps in a flower meadow, mother clapping
in the background. Camera captures the wobbling steps with gentle handheld movement.
Summer: the same child (age 5) runs through rice paddies, splashing in muddy water,
laughing freely. Golden afternoon light. Autumn: the child (age 7) walks to school with
a backpack, kicking fallen leaves on a tree-lined path. Nostalgic warm color grading.
Winter: the child (age 9) builds a snowman with siblings, breath visible in cold air.
Each season transitions through a poetic dissolve. A gentle piano melody plays throughout
with subtle environmental sounds layered underneath. Documentary voiceover tone.
Widescreen 2.39:1 cinematic aspect ratio feel.
```

</details>

<details>
<summary><b>5.3 コーヒーの朝キャンペーン</b> — ブランドストーリーテリングCM</summary>

**プロンプト：**
```
Early morning, pre-dawn blue light fills a cozy apartment. An alarm clock reads 6:00 AM.
A hand reaches out to turn it off. A woman stretches and gets out of bed. She shuffles
to the kitchen, opens a cabinet, and takes out a bag of artisan coffee beans. Close-up
of beans being poured into a grinder — the grinding sound fills the scene. She starts a
pour-over: hot water spirals over the grounds in a gooseneck kettle pour, steam rising
beautifully. The camera captures the coffee dripping in macro close-up with shallow depth
of field. She takes the first sip by the window as sunrise light breaks through. Her face
relaxes into a peaceful smile. The warmth of the coffee and sunrise blend together. Warm
color grading shifting from cool blue to golden amber. ASMR-quality sound design:
grinding, pouring water, ceramic cup sounds. End on a product shot of the coffee bag
with morning light.
```

</details>

---

### 6. 音声＆ボイス合成

Seedance 2.0 の統合音声視覚生成能力をフルに活用するプロンプト。セリフ、音楽、効果音を含みます。

| # | タイトル | 音声機能 | 難易度 | 長さ |
|:--|:--------|:--------|:-------|:-----|
| 6.1 | 猫と犬のロースト合戦 | キャラクター対話 | 上級 | 15秒 |
| 6.2 | 京劇パフォーマンス | ミュージカルボーカル | 上級 | 15秒 |
| 6.3 | シネマティック・ロードトリップMV | 音楽＋映像 | エキスパート | 20秒 |

<details>
<summary><b>6.1 猫と犬のロースト合戦</b> — リップシンク付きコメディ対話</summary>

**プロンプト：**
```
A fluffy orange cat and a golden retriever sit facing each other on a living room couch,
filmed like a reality TV confessional. The cat speaks first in a sassy, high-pitched voice:
"You know what your problem is? You get excited about EVERYTHING. A leaf blows by and
you lose your mind." The dog responds in a deep, dopey but lovable voice: "At least I
have emotions! You just sit there judging everyone like a furry little gargoyle." The cat
narrows its eyes: "I prefer the term 'sophisticated observer.'" The dog wags its tail
and pants happily: "See? That's exactly what a gargoyle would say!" Both animals have
realistic lip sync matching their dialogue. Split-screen interview format with name cards.
Sitcom-style laugh track subtly in the background. Well-lit living room, 9:16 vertical
format for social media.
```

</details>

<details>
<summary><b>6.2 京劇パフォーマンス</b> — 伝統的歌唱＋ビジュアルアート</summary>

**プロンプト：**
```
A Peking opera performer in full traditional costume and elaborate face paint (jing role,
painted face) stands center stage. Dramatic red and gold stage lighting. He begins
performing a classic aria — his voice carries the distinctive high-pitched, powerful
vibrato of Peking opera singing. The camera starts on a medium shot and slowly pushes
in to a close-up during the emotional peak of the aria. His painted expressions are
visible in detail — each gesture precise and traditional. Sleeve water sleeves flow
with his arm movements. The traditional percussion and string ensemble accompanies
his vocal. As the aria reaches its climax, the camera rotates around him in a slow
360-degree orbit. Stage smoke drifts at floor level. Dramatic theatrical lighting shifts
from warm gold to intense red at the climax. Authentic Peking opera vocal quality and
instrumentation.
```

</details>

<details>
<summary><b>6.3 シネマティック・ロードトリップMV</b> — 音楽と映像のシンクロ</summary>

**プロンプト：**
```
A cinematic music video of a solo road trip along the American Pacific Coast Highway.
The music is an upbeat indie folk song with acoustic guitar, tambourine, and warm female
vocals singing about freedom and adventure. Visual sequence synced to music beats: Verse 1
— sunrise over the ocean, a vintage red convertible cruises the coastal road, camera
mounted on the car captures the driver singing along. Chorus — rapid montage cut to the
beat: waves crashing, wind in hair, road stretching to horizon, wildflowers along the
cliff edge. Verse 2 — the car stops at a scenic overlook, the driver gets out and
stretches arms wide, camera captures from behind framing her against the vast Pacific.
Bridge — magic hour close-ups: sunlight through fingers, sand between toes on a beach,
campfire sparks at dusk. Final chorus — aerial drone shot following the car along the
serpentine highway into a spectacular sunset. The music and visuals reach a crescendo
together. Warm, nostalgic color grading throughout. 16:9 widescreen.
```

</details>

---

## プロンプトエンジニアリングのコツ

これらのテクニックを習得して、Seedance 2.0 を最大限に活用しましょう。

### カメラワークキーワード

| キーワード | 効果 | 最適な用途 |
|:----------|:-----|:----------|
| `Fixed camera` | 固定ショット | 対話シーン、商品撮影 |
| `Camera tracks` / `Tracking shot` | カメラが被写体を横方向に追う | ウォーキング、チェイス |
| `Camera pushes in` / `Push-in` | 前方ドリー移動 | 緊張感の演出、リビール |
| `Camera pulls back` / `Pullback` | 後方ドリー移動 | リビール、エスタブリッシングショット |
| `Dolly zoom` / `Hitchcock zoom` | ズーム＋逆ドリー | 心理的緊張 |
| `Orbital shot` | 被写体の360度回転 | 商品紹介、ヒーローショット |
| `Crane shot` | 垂直昇降移動 | 壮大なリビール、シーン冒頭 |
| `Whip pan` | 高速水平パン | トランジション、アクション |
| `Rack focus` / `Focus pull` | 異なる平面間のフォーカス移動 | 注目の誘導、トランジション |
| `POV shot` | 被写体の視点 | 没入体験 |
| `Aerial` / `Drone shot` | 高高度俯瞰 | 風景、エスタブリッシング |
| `Low angle` | カメラが目線以下 | 被写体を力強く見せる |
| `Dutch angle` | 傾いたフレーム | 緊張感、不安感 |

### 音声＆ボイスコントロール

> **重要な知見：** Seedance 2.0 は同一モデルパスで音声を生成します — 別途の後処理ステップではありません。これにより音声と映像のシンクロが本質的に正確です。

| テクニック | プロンプト例 |
|:----------|:-----------|
| **キャラクター対話** | `He says in a deep voice: "The time has come."` |
| **効果音** | `The sound of thunder rolls across the valley` |
| **音楽スタイル** | `Upbeat jazz piano plays in the background` |
| **環境音** | `Birds chirping, leaves rustling, distant waterfall` |
| **歌唱** | `She sings a soft lullaby in a warm soprano voice` |
| **リップシンク言語** | `She speaks in Japanese: "はじめまして"` |
| **音声トランジション** | `The busy street noise fades to peaceful silence` |
| **無音** | `Silent. No sound. Muted.` |

### マルチリファレンス技法

```
# 単一キャラクター参照
@image1 The person from the reference walks into a café...

# 複数参照の組み合わせ（人物＋商品）
@image1 @image2 The model from @image1 holds the product from @image2...

# 動画参照（動きを保持）
@video1 Recreate the movements from the reference video in a new setting...

# 複数キャラクターの一貫性
@image1 @image2 @image3 Three friends from the reference images meet at a park...
```

### 尺の最適化ガイド

| コンテンツ種別 | 推奨尺 | 理由 |
|:-------------|:------|:-----|
| 商品撮影 | 5-8秒 | 短く焦点を絞り、ループ可能 |
| SNSクリップ | 8-10秒 | Reels/TikTokの注目スパンに最適 |
| 物語シーン | 10-15秒 | ミニストーリーアークに十分 |
| 複雑なマルチショット | 15-20秒 | 3-5つの異なるショットの余地 |
| MV セグメント | 15-20秒 | フルの Aメロまたはサビ |

### アスペクト比ガイド

| 比率 | 解像度 | 最適な用途 |
|:-----|:-------|:----------|
| **16:9** | 1920x1080 | YouTube、シネマティック、横向き |
| **9:16** | 1080x1920 | TikTok、Reels、ストーリーズ |
| **1:1** | 1080x1080 | Instagram フィード、サムネイル |
| **4:3** | 1440x1080 | ヴィンテージ映画風、プレゼン |
| **3:4** | 1080x1440 | ポートレートフォト風 |

---

## 公式リソース

| リソース | リンク | 説明 |
|:---------|:------|:-----|
| ByteDance Seed | [seed.bytedance.com](https://seed.bytedance.com/) | Seed モデルファミリー公式サイト |
| 即梦 AI | [jimeng.jianying.com](https://jimeng.jianying.com/) | Seedance 公式中国語プラットフォーム |
| Seedance 論文 | [arxiv.org](https://arxiv.org/) | 統合音声視覚生成の技術論文 |
| ByteDance Research | [research.bytedance.com](https://research.bytedance.com/) | ByteDance AI 研究ポータル |

---

## コミュニティリソース

### ツール＆インテグレーション

| ツール | 説明 | リンク |
|:------|:-----|:------|
| **ComfyUI-Seedance** | Seedance の ComfyUI ノード統合 | コミュニティ GitHub |
| **Seedance Prompt Builder** | Web ベースのビジュアルプロンプトビルダー | コミュニティツール |
| **Atlas Cloud Playground** | コード不要で Seedance を実行できる Web UI | [atlascloud.ai](https://www.atlascloud.ai?ref=JPM683) |

### チュートリアル動画

- **Seedance 2.0 入門ガイド** — 基本的なプロンプト作成と生成ワークフロー
- **Seedance 高度カメラ技術** — 複雑なカメラワークの習得
- **Seedance 音声映像シンク** — 統合音声映像生成の活用
- **キャラクター一貫性マスタークラス** — 画像参照による一貫性維持
- **Seedance 商用制作** — プロフェッショナルな広告コンテンツの作成

---

## 料金比較

Seedance プロンプトを実行する最適なプラットフォームを選びましょう。

| プロバイダー | 動画あたり価格 | 速度 | 品質 | NSFW | API アクセス | 音声含む |
|:------------|:-------------|:-----|:-----|:-----|:-----------|:---------|
| **Atlas Cloud** | **$0.222** | 高速 | 最高 | 対応 | あり | あり |
| 即梦（公式） | 無料限定 | 中速 | 最高 | 非対応 | 限定 | あり |
| その他 | $0.30+ | 様々 | 様々 | 非対応 | 様々 | 様々 |

### Atlas Cloud 料金詳細

| モデル | タイプ | 価格 | 速度 |
|:------|:------|:-----|:-----|
| Seedance v1.5 Pro | テキスト→動画 | $0.222 / リクエスト | 標準 |
| Seedance v1.5 Pro | 画像→動画 | $0.222 / リクエスト | 標準 |
| Seedance v1.5 Pro Fast | テキスト→動画 | より安価 | 2倍速 |
| Seedance v1.5 Pro Fast | 画像→動画 | より安価 | 2倍速 |
| Seedance v1 Lite | テキスト→動画 | バジェット | 標準 |

> Atlas Cloud で現在 **90% 割引** 実施中。表示価格は割引後です。

---

## よくある質問

<details>
<summary><b>Seedance 2.0 とは？</b></summary>

Seedance 2.0 は ByteDance が 2026年2月にリリースした最先端の AI 動画生成モデルです。統合マルチモーダル音声視覚同時生成を実現した初の実用モデルであり、テキストプロンプトから映画品質の動画、同期音声、セリフ、音楽、マルチショット物語を単一モデルで生成します。CNN はこれを「ハリウッドを震撼させるほど強力な中国の最新 AI」と評しました。

</details>

<details>
<summary><b>Seedance 2.0 は他の AI 動画モデルとどう違う？</b></summary>

Seedance 2.0 の核心的な差別化要因は **統合マルチモーダル生成** です。競合が動画と音声を別々に生成するのに対し、Seedance 2.0 は単一モデルパスで両方を生成し、完璧なシンクロを実現します。また、複雑なカメラワーク（ドリーズーム、トラッキング、POV切替）、8言語以上の音素レベルリップシンク、マルチショット物語の一貫性をサポートしています。

</details>

<details>
<summary><b>Seedance 2.0 を最安で使う方法は？</b></summary>

最もコスト効率が良いのは [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683) で、動画あたり **$0.222**（現在90%割引実施中）です。新規ユーザーは初回チャージで **25% ボーナス** も獲得できます（最大 $100）。通常 $0.30 以上かかる他の API プロバイダーと比べて大幅に安価です。

</details>

<details>
<summary><b>Seedance 2.0 は音声やセリフを生成できる？</b></summary>

はい。Seedance 2.0 は統合音声視覚生成機能を備えています。プロンプト内で直接セリフ（8言語以上のリップシンク対応）、BGM、効果音、環境音を指定できます。モデルは同一生成パスの一部として同期音声を生成します。

</details>

<details>
<summary><b>どの解像度と尺に対応している？</b></summary>

Seedance 2.0 は最大 1080p の解像度に対応し、複数のアスペクト比（16:9、9:16、1:1、4:3、3:4）をサポートしています。動画の長さは生成ごとに 5秒から20秒の範囲です。24fps と 30fps のフレームレートに対応しています。

</details>

<details>
<summary><b>複数動画でキャラクターの一貫性を保つには？</b></summary>

リファレンスシステムを使用します：キャラクター画像をアップロードし、プロンプトで `@image1` として参照します。例：`@image1 The person from the reference walks into a café...` これにより顔の特徴、体型、主要な視覚的特徴が保持されます。`@video1` を使って前回の生成の動きとタイミングを参照することもできます。

</details>

<details>
<summary><b>リップシンクは何語に対応？</b></summary>

Seedance 2.0 は 8言語以上の音素レベルリップシンクに対応しています：英語、中国語（普通話）、日本語、韓国語、フランス語、スペイン語、ドイツ語など。プロンプト内で対象言語のセリフを書くだけで、モデルが一致するリップムーブメントを生成します。

</details>

<details>
<summary><b>商用プロジェクトに使える？</b></summary>

はい。Atlas Cloud 等のプラットフォーム経由でアクセスした場合、生成コンテンツは広告、SNSマーケティング、商品動画など商用目的に使用できます。ご利用のプラットフォームの利用規約を必ずご確認ください。

</details>

---

## スター履歴

[![Star History Chart](https://api.star-history.com/svg?repos=atlascloud/awesome-seedance-2-prompts&type=Date)](https://star-history.com/#atlascloud/awesome-seedance-2-prompts&Date)

---

## あなたのクリエイティブビジョンを実現しよう

これらのプロンプトがお気に入りですか？**Atlas Cloud** で即座に実行 — 業界で最もコスト効率の高い AI プラットフォームで、完全な創造の自由を。

| メリット | 詳細 |
|:---------|:-----|
| **無検閲 AI** | 100% の創作自由、コンテンツ制限なし |
| **最安価格** | $0.222/動画〜、90%割引適用中 |
| **高パフォーマンス** | 高速推論、キュー待ちなし |
| **25% ボーナス** | 新規ユーザーは初回チャージで最大 $100 ボーナス |
| **フル API アクセス** | REST API、Python SDK、Web プレイグラウンド |

<div align="center">

[![Atlas Cloud で生成を開始](https://img.shields.io/badge/Atlas%20Cloud%20で生成を開始-ff6b35?style=for-the-badge&logo=rocket&logoColor=white)](https://www.atlascloud.ai?ref=JPM683)

**友達紹介で初回チャージ 25% ボーナス（最大 $100）**

</div>

---

## コントリビュート

コントリビュート大歓迎です！素晴らしい Seedance 2.0 プロンプト、テクニック、リソースをお持ちの方：

1. このリポジトリを **Fork**
2. 新しいブランチを **作成** (`git checkout -b feature/my-awesome-prompt`)
3. 既存のフォーマットに従ってコンテンツを **追加**
4. 明確な説明を添えて **Pull Request を送信**

### コントリビューションガイドライン

- プロンプトは Seedance 2.0 で **テスト済み・動作確認済み** であること
- 各プロンプトに **難易度** と **推奨尺** を含める
- プロンプトが効果的な理由を説明する **コツ** を提供
- 既存のテーブルとフォーマット構造に従う
- 可能であれば全言語版（EN、ZH-CN、JA、KO）を更新

---

## ライセンス

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

このプロジェクトは MIT ライセンスの下で公開されています。詳細は [LICENSE](LICENSE) ファイルをご覧ください。

---

<div align="center">

**AI 動画生成コミュニティのために情熱を込めて作成**

このリポジトリが役立ったら、スターを付けて仲間のクリエイターにシェアしてください！

[バグ報告](https://github.com/atlascloud/awesome-seedance-2-prompts/issues) | [プロンプトリクエスト](https://github.com/atlascloud/awesome-seedance-2-prompts/issues) | [コントリビュート](https://github.com/atlascloud/awesome-seedance-2-prompts/pulls)

</div>
