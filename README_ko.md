<!--
  Awesome Seedance 2.0 프롬프트 모음
  한국어 버전
-->

<div align="center">

```
   ___                                           ___                    __                           ___      ___
  / __| ___  ___  __| | __ _  _ _   __  ___     |_  )       _ __  _ _ / _ \ _ __   _ __  | |_  ___  |_  )    / _ \
  \__ \/ -_)/ -_)/ _` |/ _` || ' \ / _|/ -_)     / /    _  | '_ \| '_| (_) | '  \ | '_ \ | __|(_-<   / / _  | (_) |
  |___/\___|\___|\__,_|\__,_||_||_|\__|\___|    /___|   (_) | .__/|_|  \___/|_|_|_|| .__/ |_|  /__/  /___(_)  \___/
                                                            |_|                    |_|
```

# Awesome Seedance 2.0 프롬프트 모음

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/atlascloud/awesome-seedance-2-prompts?style=social)](https://github.com/atlascloud/awesome-seedance-2-prompts/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Last Commit](https://img.shields.io/github/last-commit/atlascloud/awesome-seedance-2-prompts)](https://github.com/atlascloud/awesome-seedance-2-prompts/commits/main)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/atlascloud/awesome-seedance-2-prompts/pulls)
[![Seedance](https://img.shields.io/badge/Seedance-2.0-blue?logo=bytedance&logoColor=white)](https://seed.bytedance.com/)
[![Atlas Cloud](https://img.shields.io/badge/지금%20사용-Atlas%20Cloud-orange)](https://www.atlascloud.ai?ref=JPM683)

**ByteDance의 Seedance 2.0을 위한 고품질 프롬프트, 팁, 리소스의 엄선된 컬렉션 — 세계에서 가장 진보된 통합 멀티모달 AI 동영상 생성 모델.**

CNN은 이를 **"할리우드를 공포에 떨게 할 만큼 강력한 중국의 최신 AI"** 라고 평가했습니다.

[English](README.md) | [中文](README_zh-CN.md) | [日本語](README_ja.md) | [한국어](README_ko.md)

---

**유용하다면 이 저장소에 스타를 눌러주세요!** 여러분의 지지가 더 많은 크리에이터에게 이 리소스를 전달합니다.

</div>

---

<div align="center">

### Atlas Cloud에서 이 프롬프트를 즉시 실행하세요

Seedance 2.0을 최고 품질로 체험하는 가장 빠르고 저렴한 방법.

**무검열 AI** | **최저가 $0.222/초부터** | **2배 빠른 추론**

[![Atlas Cloud 사용해보기](https://img.shields.io/badge/Atlas%20Cloud%20사용해보기-무료%20시작-ff6b35?style=for-the-badge&logo=rocket&logoColor=white)](https://www.atlascloud.ai?ref=JPM683)

신규 사용자 첫 충전 시 **25% 보너스** 지급 (최대 $100)

</div>

> 🔒 **엔터프라이즈급 보안** — Atlas Cloud는 **SOC I & II 인증** | **HIPAA 준수** | 미국 기업, 99.9% 가동률 SLA 보장.

> 🎨 **NSFW 화이트리스트 업데이트** — Seedance와 Kling 외에도 **Vidu 시리즈** (Q3-Pro, Q3-Turbo)가 Atlas Cloud의 무검열 콘텐츠 생성 화이트리스트에 추가되었습니다.

---

## 목차

- [Seedance 2.0 소개](#seedance-20-소개)
- [빠른 시작 (API)](#빠른-시작-api)
- [프롬프트 모음](#프롬프트-모음)
  - [초사실적 동영상 생성](#1-초사실적-동영상-생성)
  - [캐릭터 및 장면 일관성](#2-캐릭터-및-장면-일관성)
  - [고급 카메라 움직임](#3-고급-카메라-움직임)
  - [창의적 시각 효과](#4-창의적-시각-효과)
  - [스토리 전개 및 확장](#5-스토리-전개-및-확장)
  - [오디오 및 음성 합성](#6-오디오-및-음성-합성)
- [프롬프트 엔지니어링 팁](#프롬프트-엔지니어링-팁)
- [공식 리소스](#공식-리소스)
- [커뮤니티 리소스](#커뮤니티-리소스)
- [가격 비교](#가격-비교)
- [자주 묻는 질문](#자주-묻는-질문)
- [스타 히스토리](#스타-히스토리)
- [기여하기](#기여하기)
- [라이선스](#라이선스)

---

## Seedance 2.0 소개

**Seedance 2.0**은 ByteDance가 **2026년 2월**에 출시한 차세대 AI 동영상 생성 모델입니다. **통합 멀티모달 오디오-비주얼 동시 생성**을 단일 아키텍처로 실현한 최초의 프로덕션 모델로, 하나의 프롬프트로 시네마틱 동영상, 동기화된 오디오, 대사, 음악, 멀티샷 내러티브를 생성합니다.

### 핵심 기능

| 기능 | 상세 |
|:-----|:-----|
| **통합 오디오-비주얼 생성** | 단일 모델이 동영상 + 동기화 오디오 + 대사를 한 번에 생성 |
| **복잡한 카메라 움직임** | 푸시풀 줌, 포커스 전환, 트래킹 샷, POV 전환, 히치콕 줌 등 |
| **멀티샷 내러티브** | 캐릭터와 장면 일관성을 유지하는 연속 멀티샷 시퀀스 생성 |
| **8개 이상 언어 립싱크** | 한국어, 영어, 중국어, 일본어 등 8개 이상 언어의 음소 수준 립싱크 |
| **캐릭터 일관성** | 이미지/동영상 참조(`@image1`, `@video1`)로 샷 간 캐릭터 일관성 유지 |
| **시네마틱 품질** | 할리우드급 비주얼 품질, 사실적인 조명, 피사계 심도, 모션 블러 |

### 주요 사양

| 사양 | 값 |
|:-----|:---|
| 최대 해상도 | 최대 1080p |
| 동영상 길이 | 생성당 5초~20초 |
| 화면비 | 16:9, 9:16, 1:1, 4:3, 3:4 |
| 오디오 | 스테레오 |
| 프레임율 | 24fps / 30fps |
| 입력 모드 | 텍스트→동영상, 이미지→동영상, 동영상→동영상 |
| 참조 지원 | 다중 이미지(`@image1`, `@image2`), 동영상 참조(`@video1`) |

### 활용 사례

- **영화 제작 및 프리비즈** — 스토리보드를 동영상으로 빠르게 변환, 컨셉 시각화, VFX 프리뷰
- **광고 및 마케팅** — 제품 광고, 브랜드 캠페인, SNS 광고
- **SNS 및 UGC** — 숏폼 콘텐츠, TikTok/릴스, 크리에이티브 스토리텔링
- **이커머스** — 제품 쇼케이스 동영상, 가상 피팅, 라이프스타일 데모
- **교육 및 훈련** — 설명 동영상, 역사 재현, 과학 시각화
- **음악 및 엔터테인먼트** — 뮤직비디오, 가사 동영상, 콘서트 비주얼

---

## 빠른 시작 (API)

Atlas Cloud의 API로 몇 초 만에 Seedance 2.0을 실행하세요. GPU 설정이 필요 없습니다.

### API 키 발급

1. [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)에서 가입
2. 대시보드의 **API Keys** 메뉴로 이동
3. 새 키를 생성하고 복사

### cURL 예제

```bash
# Atlas Cloud API로 Seedance 2.0 동영상 생성 호출
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

### Python 예제

```python
import requests
import time

# Atlas Cloud API 설정
API_KEY = "YOUR_API_KEY"
BASE_URL = "https://api.atlascloud.ai/api/v1/model"

def generate_video(prompt: str, duration: int = 10, aspect_ratio: str = "16:9"):
    """
    Seedance 2.0 모델로 동영상을 생성합니다

    매개변수:
        prompt: 동영상 생성 프롬프트
        duration: 동영상 길이(초)
        aspect_ratio: 동영상 화면비
    반환:
        동영상 생성 태스크의 결과
    """
    # 동영상 생성 요청 제출
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
    print(f"태스크 제출 완료, ID: {task_id}")

    # 생성 상태 폴링 확인
    while True:
        status_resp = requests.get(
            f"{BASE_URL}/task/{task_id}",
            headers={"Authorization": f"Bearer {API_KEY}"}
        )
        status = status_resp.json()

        if status["status"] == "completed":
            print("동영상 생성 완료!")
            return status["output"]["video_url"]
        elif status["status"] == "failed":
            raise Exception(f"생성 실패: {status.get('error')}")

        time.sleep(5)  # 5초마다 상태 확인

# 사용 예시
video_url = generate_video(
    prompt="Camera slightly pulls back revealing the full street view and follows "
           "the female protagonist moving. The wind blows the hem of her dress as "
           "she walks on the streets of 19th century London. Cinematic lighting, "
           "film grain, anamorphic lens.",
    duration=15,
    aspect_ratio="16:9"
)
print(f"동영상 다운로드 URL: {video_url}")
```

---

## 프롬프트 모음

> **사용법**: 아래의 프롬프트를 복사하여 [Atlas Cloud 플레이그라운드](https://www.atlascloud.ai?ref=JPM683)에 직접 붙여넣거나 API로 사용하세요. `@image1` 또는 `@video1`이 포함된 프롬프트는 참조 이미지/동영상을 먼저 업로드하세요.

---

### 1. 초사실적 동영상 생성

사실적인 동영상 출력을 위한 프롬프트. 자연스러운 동작과 시네마틱 품질을 갖추고 있습니다.

| # | 제목 | 난이도 | 길이 | 화면비 |
|:--|:-----|:-------|:-----|:-------|
| 1.1 | 우아한 빨래 장면 | 초급 | 10초 | 16:9 |
| 1.2 | 인터랙티브 그림 캐릭터 | 중급 | 10초 | 9:16 |
| 1.3 | 빅토리아 시대 거리 풍경 | 중급 | 15초 | 16:9 |
| 1.4 | 장애물 추격 장면 | 고급 | 15초 | 16:9 |

<details>
<summary><b>1.1 우아한 빨래 장면</b> — 자연스러운 물리 시뮬레이션의 고요한 일상</summary>

**프롬프트:**
```
Fixed camera shot, a girl elegantly hanging clothes to dry, after finishing she takes out
another piece from the basket and shakes the clothes vigorously. The fabric flows naturally
in the breeze. Sunlight filters through the wet fabric creating beautiful light diffusion.
Warm afternoon lighting, shallow depth of field, 4K cinematic quality.
```

**팁:**
- "Fixed camera" 지시로 샷을 안정시키고 피사체의 움직임에 집중
- "shakes the clothes vigorously"가 Seedance 2.0의 물리 시뮬레이션 능력을 테스트
- 빛의 상호작용 디테일("sunlight filters through") 추가로 사실감 향상

</details>

<details>
<summary><b>1.2 인터랙티브 그림 캐릭터</b> — 제4의 벽을 깨는 회화 예술</summary>

**프롬프트:**
```
The character in the painting has a guilty expression, eyes looking left and right, then
peeks out of the frame, quickly extends their hand out of the frame to grab a cola and
takes a sip. After drinking, they let out a satisfied sigh, wipe their mouth, and retreat
back into the painting, resuming their original elegant pose as if nothing happened.
Oil painting style blending with photorealistic elements. Warm gallery lighting.
```

**팁:**
- 이 프롬프트는 예술적 스타일과 사실주의를 융합하는 Seedance 2.0의 능력을 보여줌
- 연속 동작(엿보기, 잡기, 마시기, 돌아가기)이 시간적 일관성을 테스트
- SNS 콘텐츠에 최적 — 공유성이 높고 매력적

</details>

<details>
<summary><b>1.3 빅토리아 시대 거리 풍경</b> — 트래킹이 있는 시대극 시네마토그래피</summary>

**프롬프트:**
```
Camera slightly pulls back (revealing the full street view) and follows the female
protagonist moving. The wind blows the hem of her dress as she walks on the streets
of 19th century London. Gas lamps flicker along cobblestone streets. Horse-drawn
carriages pass in the background. Pedestrians in period-appropriate attire populate
the scene. Fog rolls gently through the narrow lanes. Cinematic color grading with
desaturated tones, film grain, anamorphic lens flare. 4K resolution.
```

**팁:**
- 카메라 풀백 + 트래킹으로 다이내믹하고 전문적인 카메라워크 구현
- 시대별 디테일(가스등, 자갈길, 마차)이 모델을 정확하게 가이드
- "아나모픽 렌즈 플레어"와 "필름 그레인"으로 영화적 품질 추가

</details>

<details>
<summary><b>1.4 장애물 추격 장면</b> — 다중 캐릭터 빠른 속도 액션</summary>

**프롬프트:**
```
Camera follows a man in black clothes fleeing quickly through a crowded marketplace,
with a group of people chasing behind. He knocks over fruit stalls, ducks under hanging
fabrics, and leaps over a cart. The chasers stumble over the obstacles he leaves behind.
Handheld camera feel with slight shake. Fast-paced editing rhythm. Dramatic shadows and
high contrast lighting. Urban environment, daytime. Cinematic action movie style.
```

**팁:**
- 다중 캐릭터 상호작용이 모델의 공간 추론 능력을 테스트
- 환경 파괴(노점 넘어뜨리기)가 다이내믹한 복잡성 추가
- "핸드헬드 카메라 느낌"으로 정통 액션 영화 미학 연출

</details>

---

### 2. 캐릭터 및 장면 일관성

참조 이미지와 동영상(`@image1`, `@video1`)을 활용하여 캐릭터 정체성과 장면 연속성을 유지하는 프롬프트.

| # | 제목 | 참조 유형 | 난이도 | 길이 |
|:--|:-----|:---------|:-------|:-----|
| 2.1 | 퇴근 후 귀가 | `@image1` | 중급 | 10초 |
| 2.2 | 경극 무대 전환 | `@video1` | 고급 | 15초 |
| 2.3 | 원테이크 심리스 전환 | 없음 | 고급 | 20초 |
| 2.4 | 럭셔리 핸드백 광고 | `@image1` + `@image2` | 중급 | 10초 |

<details>
<summary><b>2.1 퇴근 후 귀가</b> — 참조 이미지 기반 일관된 캐릭터</summary>

**프롬프트:**
```
@image1 The woman in the reference image arrives home after a long day at work. She opens
the front door, drops her bag on the hallway table, kicks off her heels, and walks to the
kitchen. She opens the refrigerator, the cool light illuminates her tired but content face.
She grabs a bottle of water and takes a long sip. Warm interior lighting transitioning to
cool refrigerator light. Cinematic, intimate atmosphere. 16:9 aspect ratio.
```

**팁:**
- `@image1`이 캐릭터의 얼굴, 헤어스타일, 체형을 유지
- 연속 장면 전환(복도→주방→냉장고)이 공간 일관성을 테스트
- 장면 전체의 조명 변화가 제작 가치를 높임

</details>

<details>
<summary><b>2.2 경극 무대 전환</b> — 동영상 참조 기반 스타일 전환</summary>

**프롬프트:**
```
@video1 Transform this performance into a grand Chinese opera stage setting. The performer
maintains the same movements and expressions from the reference video, but is now wearing
elaborate Peking opera costume with ornate headdress. The stage features traditional red
and gold decorations, dramatic theatrical lighting with colored spotlights. Smoke effects
drift across the stage floor. Traditional Chinese instrumental accompaniment plays in sync
with the movements. Cinematic wide shot gradually pushing in to medium close-up.
```

**팁:**
- `@video1`이 참조 동영상의 동작과 타이밍을 보존
- 현대에서 전통 경극으로의 스타일 전환이 모델의 창작 범위를 테스트
- 오디오 생성이 시각적 전환과 동기화되도록 지정

</details>

<details>
<summary><b>2.3 원테이크 심리스 전환</b> — 복잡한 연속 촬영</summary>

**프롬프트:**
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

**팁:**
- Seedance 2.0의 공간 전환 능력을 테스트하는 고급 프롬프트
- "No cuts"와 "seamless"가 연속성 유지를 위한 핵심 지시
- 각 환경마다 고유한 조명과 분위기가 매끄럽게 전환되어야 함
- 권장 길이: 완전한 효과를 위해 20초

</details>

<details>
<summary><b>2.4 럭셔리 핸드백 광고</b> — 이중 참조의 제품 포커스 광고</summary>

**프롬프트:**
```
@image1 @image2 A luxury fashion commercial. The model from @image1 carries the handbag
from @image2. She walks confidently down a marble hallway in a grand European hotel.
Camera tracks alongside her at waist level, keeping the handbag in focus. She pauses at
a large window, golden hour light streams in, illuminating the bag's leather texture and
metallic hardware. She runs her fingers along the bag's stitching. Shallow depth of field,
the background softly blurs. Cut to a tabletop shot of the bag alone on a velvet surface
with dramatic side lighting. Premium commercial quality, 4K.
```

**팁:**
- 이중 참조(`@image1` 모델용, `@image2` 제품용)로 정밀한 브랜드 제어
- 허리 높이 카메라로 제품이 항상 눈에 띄게 유지
- 골든아워 + 얕은 피사계 심도는 럭셔리 제품 촬영의 성공 공식

</details>

---

### 3. 고급 카메라 움직임

Seedance 2.0의 업계 최고 수준 카메라 제어 능력을 보여주는 프롬프트.

| # | 제목 | 카메라 기법 | 난이도 | 길이 |
|:--|:-----|:----------|:-------|:-----|
| 3.1 | 엘리베이터 히치콕 줌 | 돌리 줌 (현기증 효과) | 고급 | 10초 |
| 3.2 | 복도 복합 추격 | 트래킹 + 포커스 풀 | 고급 | 15초 |
| 3.3 | 자동차 CF 시네마토그래피 | 오비탈 + 크레인 + 트래킹 | 전문가 | 15초 |
| 3.4 | 무술 격투 장면 | 다이내믹 다중 앵글 | 고급 | 10초 |

<details>
<summary><b>3.1 엘리베이터 히치콕 줌</b> — 클래식 현기증/돌리 줌 효과</summary>

**프롬프트:**
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
<summary><b>3.2 복도 복합 추격</b> — 멀티 테크닉 트래킹 샷</summary>

**프롬프트:**
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
<summary><b>3.3 자동차 CF 시네마토그래피</b> — 프리미엄 자동차 영상</summary>

**프롬프트:**
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
<summary><b>3.4 무술 격투 장면</b> — 다이내믹 액션 시네마토그래피</summary>

**프롬프트:**
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

### 4. 창의적 시각 효과

Seedance 2.0의 초현실적, 예술적, 이펙트 중심 콘텐츠 생성 능력을 탐구하는 프롬프트.

| # | 제목 | 스타일 | 난이도 | 길이 |
|:--|:-----|:-------|:-------|:-----|
| 4.1 | VR 안경 우주 여행 | SF / 초현실 | 고급 | 15초 |
| 4.2 | 패션 빠른 의상 변환 CF | 패션 / VFX | 중급 | 10초 |
| 4.3 | 수묵화 태극권 | 전통 예술 / 모션 | 중급 | 15초 |
| 4.4 | 마법 변신 시퀀스 | 판타지 / VFX | 고급 | 10초 |
| 4.5 | 골드 파티클 타이틀 공개 | 모션 그래픽스 / VFX | 중급 | 8초 |

<details>
<summary><b>4.1 VR 안경 우주 여행</b> — 몰입형 SF 비주얼라이제이션</summary>

**프롬프트:**
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
<summary><b>4.2 패션 빠른 의상 변환 CF</b> — 빠른 의상 전환</summary>

**프롬프트:**
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
<summary><b>4.3 수묵화 태극권</b> — 중국 전통 예술의 모션 표현</summary>

**프롬프트:**
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
<summary><b>4.4 마법 변신 시퀀스</b> — 판타지 변신</summary>

**프롬프트:**
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
<summary><b>4.5 골드 파티클 타이틀 공개</b> — 모션 그래픽스 타이틀 시퀀스</summary>

**프롬프트:**
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

### 5. 스토리 전개 및 확장

명확한 스토리 아크를 가진 내러티브 중심 동영상 콘텐츠 프롬프트.

| # | 제목 | 내러티브 유형 | 난이도 | 길이 |
|:--|:-----|:------------|:-------|:-----|
| 5.1 | 만화 패널 애니메이션 | 연속 내러티브 | 중급 | 15초 |
| 5.2 | 어린 시절 사계절 다큐멘터리 | 다큐멘터리 몽타주 | 고급 | 20초 |
| 5.3 | 커피 모닝 캠페인 | 브랜드 스토리 | 초급 | 10초 |

<details>
<summary><b>5.1 만화 패널 애니메이션</b> — 정적 패널에 생명을 불어넣다</summary>

**프롬프트:**
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
<summary><b>5.2 어린 시절 사계절 다큐멘터리</b> — 감동적인 타임랩스 내러티브</summary>

**프롬프트:**
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
<summary><b>5.3 커피 모닝 캠페인</b> — 브랜드 스토리텔링 광고</summary>

**프롬프트:**
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

### 6. 오디오 및 음성 합성

Seedance 2.0의 통합 오디오-비주얼 생성 능력을 최대한 활용하는 프롬프트. 대사, 음악, 효과음 포함.

| # | 제목 | 오디오 기능 | 난이도 | 길이 |
|:--|:-----|:----------|:-------|:-----|
| 6.1 | 고양이와 강아지 디스전 | 캐릭터 대화 | 고급 | 15초 |
| 6.2 | 경극 퍼포먼스 | 뮤지컬 보컬 | 고급 | 15초 |
| 6.3 | 시네마틱 로드트립 MV | 음악 + 영상 | 전문가 | 20초 |

<details>
<summary><b>6.1 고양이와 강아지 디스전</b> — 립싱크 포함 코미디 대화</summary>

**프롬프트:**
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
<summary><b>6.2 경극 퍼포먼스</b> — 전통 성악 + 시각 예술</summary>

**프롬프트:**
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
<summary><b>6.3 시네마틱 로드트립 MV</b> — 음악과 영상의 싱크로</summary>

**프롬프트:**
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

## 프롬프트 엔지니어링 팁

이 테크닉들을 습득하여 Seedance 2.0의 잠재력을 최대한 발휘하세요.

### 카메라 움직임 키워드

| 키워드 | 효과 | 적합한 용도 |
|:-------|:-----|:-----------|
| `Fixed camera` | 고정 샷, 움직임 없음 | 대화 장면, 제품 촬영 |
| `Camera tracks` / `Tracking shot` | 카메라가 피사체를 횡방향으로 추적 | 워킹, 추격 장면 |
| `Camera pushes in` / `Push-in` | 전방 돌리 이동 | 긴장감 조성, 리빌 |
| `Camera pulls back` / `Pullback` | 후방 돌리 이동 | 리빌, 이스태블리싱 샷 |
| `Dolly zoom` / `Hitchcock zoom` | 줌 + 역방향 돌리 | 심리적 긴장감 |
| `Orbital shot` | 피사체 360도 회전 | 제품 쇼케이스, 히어로 샷 |
| `Crane shot` | 수직 상승/하강 이동 | 웅장한 리빌, 장면 도입 |
| `Whip pan` | 빠른 수평 팬 | 전환, 액션 장면 |
| `Rack focus` / `Focus pull` | 서로 다른 평면 간 포커스 이동 | 주의 유도, 전환 |
| `POV shot` | 피사체의 시점 | 몰입 경험 |
| `Aerial` / `Drone shot` | 고고도 조감 | 풍경, 이스태블리싱 |
| `Low angle` | 카메라가 눈높이 아래 | 피사체를 강력하게 표현 |
| `Dutch angle` | 기울어진 프레임 | 긴장감, 불안감 |

### 오디오 및 음성 제어

> **핵심 포인트:** Seedance 2.0은 동일한 모델 패스에서 오디오를 생성합니다 — 별도의 후처리 단계가 아닙니다. 이는 오디오-비주얼 동기화가 본질적으로 정확함을 의미합니다.

| 테크닉 | 프롬프트 예시 |
|:-------|:------------|
| **캐릭터 대화** | `He says in a deep voice: "The time has come."` |
| **효과음** | `The sound of thunder rolls across the valley` |
| **음악 스타일** | `Upbeat jazz piano plays in the background` |
| **환경음** | `Birds chirping, leaves rustling, distant waterfall` |
| **보컬** | `She sings a soft lullaby in a warm soprano voice` |
| **립싱크 언어** | `She speaks in Korean: "안녕하세요"` |
| **오디오 전환** | `The busy street noise fades to peaceful silence` |
| **무음** | `Silent. No sound. Muted.` |

### 멀티 레퍼런스 기법

```
# 단일 캐릭터 참조
@image1 The person from the reference walks into a café...

# 다중 참조 조합 (인물 + 제품)
@image1 @image2 The model from @image1 holds the product from @image2...

# 동영상 참조 (동작 유지)
@video1 Recreate the movements from the reference video in a new setting...

# 다중 캐릭터 일관성
@image1 @image2 @image3 Three friends from the reference images meet at a park...
```

### 길이 최적화 가이드

| 콘텐츠 유형 | 권장 길이 | 이유 |
|:-----------|:---------|:-----|
| 제품 촬영 | 5-8초 | 짧고 집중적, 루프 가능 |
| SNS 클립 | 8-10초 | 릴스/TikTok 주의 지속 시간에 최적 |
| 내러티브 장면 | 10-15초 | 미니 스토리 아크에 충분 |
| 복잡한 멀티샷 | 15-20초 | 3-5개의 다른 샷 여유 |
| MV 세그먼트 | 15-20초 | 풀 벌스 또는 코러스 |

### 화면비 가이드

| 비율 | 해상도 | 적합한 용도 |
|:-----|:-------|:-----------|
| **16:9** | 1920x1080 | YouTube, 시네마틱, 가로 |
| **9:16** | 1080x1920 | TikTok, 릴스, 스토리 |
| **1:1** | 1080x1080 | Instagram 피드, 썸네일 |
| **4:3** | 1440x1080 | 빈티지 영화 느낌, 프레젠테이션 |
| **3:4** | 1080x1440 | 인물 사진 스타일 |

---

## 공식 리소스

| 리소스 | 링크 | 설명 |
|:-------|:-----|:-----|
| ByteDance Seed | [seed.bytedance.com](https://seed.bytedance.com/) | Seed 모델 패밀리 공식 홈페이지 |
| 즉몽 AI | [jimeng.jianying.com](https://jimeng.jianying.com/) | Seedance 공식 중국어 플랫폼 |
| Seedance 논문 | [arxiv.org](https://arxiv.org/) | 통합 오디오-비주얼 생성 기술 논문 |
| ByteDance Research | [research.bytedance.com](https://research.bytedance.com/) | ByteDance AI 연구 포탈 |

---

## 커뮤니티 리소스

### 도구 및 통합

| 도구 | 설명 | 링크 |
|:-----|:-----|:-----|
| **ComfyUI-Seedance** | Seedance의 ComfyUI 노드 통합 | 커뮤니티 GitHub |
| **Seedance Prompt Builder** | 웹 기반 비주얼 프롬프트 빌더 | 커뮤니티 도구 |
| **Atlas Cloud Playground** | 코드 없이 Seedance를 실행하는 Web UI | [atlascloud.ai](https://www.atlascloud.ai?ref=JPM683) |

### 튜토리얼 동영상

- **Seedance 2.0 시작 가이드** — 기본 프롬프트 작성 및 생성 워크플로우
- **Seedance 고급 카메라 기법** — 복잡한 카메라 움직임 마스터
- **Seedance 오디오-비주얼 싱크** — 통합 오디오-비디오 생성 활용
- **캐릭터 일관성 마스터클래스** — 이미지 참조로 일관된 캐릭터 유지
- **Seedance 상업 제작** — 전문적인 광고 콘텐츠 제작

---

## 가격 비교

Seedance 프롬프트를 실행할 최적의 플랫폼을 선택하세요.

| 제공업체 | 동영상당 가격 | 속도 | 품질 | NSFW | API 접근 | 오디오 포함 |
|:---------|:------------|:-----|:-----|:-----|:--------|:----------|
| **Atlas Cloud** | **$0.222** | 빠름 | 최상 | 지원 | 있음 | 있음 |
| 즉몽(공식) | 무료 제한 | 보통 | 최상 | 미지원 | 제한적 | 있음 |
| 기타 | $0.30+ | 다양 | 다양 | 미지원 | 다양 | 다양 |

### Atlas Cloud 상세 가격

| 모델 | 유형 | 가격 | 속도 |
|:-----|:-----|:-----|:-----|
| Seedance v1.5 Pro | 텍스트→동영상 | $0.222 / 요청 | 표준 |
| Seedance v1.5 Pro | 이미지→동영상 | $0.222 / 요청 | 표준 |
| Seedance v1.5 Pro Fast | 텍스트→동영상 | 더 저렴 | 2배속 |
| Seedance v1.5 Pro Fast | 이미지→동영상 | 더 저렴 | 2배속 |
| Seedance v1 Lite | 텍스트→동영상 | 저예산 | 표준 |

> Atlas Cloud에서 현재 **90% 할인** 진행 중. 표시된 가격은 할인 후 가격입니다.

### Atlas Cloud vs fal.ai 가격 비교

| 모델 | fal.ai 가격 | Atlas Cloud 가격 | 절약 |
|:------|:------------|:-----------------|:---------|
| **Kling** | $0.224/초 (5초 = $1.12) | $0.204/초부터 | **82% 저렴** |
| **Seedance** | ~$0.26/영상 | $0.222/초부터 | **15% 저렴** |
| **Wan 2.5** | $0.05/초 (5초 = $0.25) | $0.05/초부터 | **80% 저렴** |
| **Wan 2.6** | 유사 가격 | $0.07/초부터 | 경쟁력 있음 |
| **Veo 3** | $0.40/초 (8초 = $3.20) | 출시 예정 | 준비 중 |
| **Vidu Q3-Pro** | — | $0.06/초부터 | Atlas 독점 |
| **Vidu Q3-Turbo** | — | $0.034/초부터 | Atlas 독점 |

*표시된 가격은 시작 가격입니다. 더 높은 해상도나 긴 영상은 추가 비용이 발생할 수 있습니다.*

> 💡 Atlas Cloud는 모든 주요 영상 모델에서 **최저가**를 제공합니다. fal.ai에서 전환하면 영상 생성 비용을 최대 **82%** 절약할 수 있습니다.

---

## 자주 묻는 질문

<details>
<summary><b>Seedance 2.0이란?</b></summary>

Seedance 2.0은 ByteDance가 2026년 2월에 출시한 최첨단 AI 동영상 생성 모델입니다. 통합 멀티모달 오디오-비주얼 동시 생성을 실현한 최초의 프로덕션 모델로, 텍스트 프롬프트에서 시네마틱 동영상, 동기화된 오디오, 대사, 음악, 멀티샷 내러티브를 단일 모델로 생성합니다. CNN은 이를 "할리우드를 공포에 떨게 할 만큼 강력한 중국의 최신 AI"라고 평가했습니다.

</details>

<details>
<summary><b>Seedance 2.0은 다른 AI 동영상 모델과 어떻게 다른가?</b></summary>

Seedance 2.0의 핵심 차별점은 **통합 멀티모달 생성**입니다. 경쟁 모델들이 동영상과 오디오를 별도로 생성하는 반면, Seedance 2.0은 단일 모델 패스에서 둘 다 생성하여 완벽한 동기화를 보장합니다. 또한 복잡한 카메라 움직임(돌리 줌, 트래킹, POV 전환), 8개 이상 언어의 음소 수준 립싱크, 멀티샷 내러티브 일관성을 지원합니다.

</details>

<details>
<summary><b>Seedance 2.0을 가장 저렴하게 사용하는 방법은?</b></summary>

가장 비용 효율적인 방법은 [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)로, 동영상당 **$0.222** (현재 90% 할인 적용)입니다. 신규 사용자는 첫 충전 시 **25% 보너스** (최대 $100)도 받을 수 있습니다. 일반적으로 $0.30 이상을 부과하는 다른 API 제공업체보다 훨씬 저렴합니다.

</details>

<details>
<summary><b>Seedance 2.0은 오디오와 대사를 생성할 수 있나?</b></summary>

네. Seedance 2.0은 통합 오디오-비주얼 생성 기능을 갖추고 있습니다. 프롬프트에서 직접 대사(8개 이상 언어 립싱크 지원), 배경 음악, 효과음, 환경음을 지정할 수 있습니다. 모델은 동일한 생성 패스의 일부로 동기화된 오디오를 생성합니다.

</details>

<details>
<summary><b>어떤 해상도와 길이를 지원하나?</b></summary>

Seedance 2.0은 최대 1080p 해상도와 다양한 화면비(16:9, 9:16, 1:1, 4:3, 3:4)를 지원합니다. 동영상 길이는 생성당 5초에서 20초 범위입니다. 24fps와 30fps 프레임율을 지원합니다.

</details>

<details>
<summary><b>여러 동영상에서 캐릭터 일관성을 유지하려면?</b></summary>

레퍼런스 시스템을 사용합니다: 캐릭터 이미지를 업로드하고 프롬프트에서 `@image1`로 참조합니다. 예: `@image1 The person from the reference walks into a café...` 이렇게 하면 얼굴 특징, 체형, 주요 시각적 특성이 유지됩니다. `@video1`을 사용하여 이전 생성의 동작과 타이밍을 참조할 수도 있습니다.

</details>

<details>
<summary><b>립싱크는 몇 개 언어를 지원하나?</b></summary>

Seedance 2.0은 8개 이상 언어의 음소 수준 립싱크를 지원합니다: 영어, 중국어(보통화), 일본어, 한국어, 프랑스어, 스페인어, 독일어 등. 프롬프트에서 대상 언어로 대사를 작성하면 모델이 일치하는 입 모양을 생성합니다.

</details>

<details>
<summary><b>상업 프로젝트에 사용할 수 있나?</b></summary>

네. Atlas Cloud 등의 플랫폼을 통해 접근할 경우, 생성된 콘텐츠는 광고, SNS 마케팅, 제품 동영상 등 상업적 목적으로 사용할 수 있습니다. 사용하시는 플랫폼의 이용약관을 반드시 확인하세요.

</details>

---

## 스타 히스토리

[![Star History Chart](https://api.star-history.com/svg?repos=atlascloud/awesome-seedance-2-prompts&type=Date)](https://star-history.com/#atlascloud/awesome-seedance-2-prompts&Date)

---

## 창의적 비전을 현실로 만드세요

이 프롬프트들이 마음에 드셨나요? **Atlas Cloud**에서 즉시 실행하세요 — 업계에서 가장 비용 효율적인 AI 플랫폼으로, 완전한 창작 자유를 누리세요.

| 혜택 | 상세 |
|:-----|:-----|
| **무검열 AI** | 100% 창작 자유, 콘텐츠 제한 없음 |
| **최저 가격** | $0.222/초부터, 90% 할인 적용 |
| **고성능** | 빠른 추론, 대기 없음 |
| **25% 보너스** | 신규 사용자 첫 충전 시 최대 $100 보너스 |
| **풀 API 접근** | REST API, Python SDK, 웹 플레이그라운드 |

<div align="center">

[![Atlas Cloud에서 생성 시작](https://img.shields.io/badge/Atlas%20Cloud에서%20생성%20시작-ff6b35?style=for-the-badge&logo=rocket&logoColor=white)](https://www.atlascloud.ai?ref=JPM683)

**친구 추천 시 첫 충전 25% 보너스 (최대 $100)**

</div>

---

## 기여하기

기여를 환영합니다! 훌륭한 Seedance 2.0 프롬프트, 팁, 리소스를 공유하고 싶으시다면:

1. 이 저장소를 **Fork**
2. 새 브랜치 **생성** (`git checkout -b feature/my-awesome-prompt`)
3. 기존 형식에 따라 콘텐츠 **추가**
4. 명확한 설명과 함께 **Pull Request 제출**

### 기여 가이드라인

- 프롬프트는 Seedance 2.0에서 **테스트 및 검증 완료**되어야 함
- 각 프롬프트에 **난이도**와 **권장 길이** 포함
- 프롬프트가 효과적인 이유를 설명하는 **팁** 제공
- 기존 테이블 및 포맷 구조를 따름
- 가능하면 모든 언어 버전(EN, ZH-CN, JA, KO) 업데이트

---

## 라이선스

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

이 프로젝트는 MIT 라이선스 하에 공개되어 있습니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

---

<div align="center">

**AI 동영상 생성 커뮤니티를 위해 열정을 담아 제작**

이 저장소가 도움이 되었다면, 스타를 누르고 동료 크리에이터들에게 공유해주세요!

[버그 리포트](https://github.com/atlascloud/awesome-seedance-2-prompts/issues) | [프롬프트 요청](https://github.com/atlascloud/awesome-seedance-2-prompts/issues) | [기여하기](https://github.com/atlascloud/awesome-seedance-2-prompts/pulls)

</div>
