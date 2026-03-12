<!--
  Awesome Seedance 2.0 Prompts
  精心整理的 Seedance 2.0 提示词集合
-->

<div align="center">

```
   ___                                           ___                    __                           ___      ___
  / __| ___  ___  __| | __ _  _ _   __  ___     |_  )       _ __  _ _ / _ \ _ __   _ __  | |_  ___  |_  )    / _ \
  \__ \/ -_)/ -_)/ _` |/ _` || ' \ / _|/ -_)     / /    _  | '_ \| '_| (_) | '  \ | '_ \ | __|(_-<   / / _  | (_) |
  |___/\___|\___|\__,_|\__,_||_||_|\__|\___|    /___|   (_) | .__/|_|  \___/|_|_|_|| .__/ |_|  /__/  /___(_)  \___/
                                                            |_|                    |_|
```

# Awesome Seedance 2.0 Prompts

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/atlascloud/awesome-seedance-2-prompts?style=social)](https://github.com/atlascloud/awesome-seedance-2-prompts/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Last Commit](https://img.shields.io/github/last-commit/atlascloud/awesome-seedance-2-prompts)](https://github.com/atlascloud/awesome-seedance-2-prompts/commits/main)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/atlascloud/awesome-seedance-2-prompts/pulls)
[![Seedance](https://img.shields.io/badge/Seedance-2.0-blue?logo=bytedance&logoColor=white)](https://seed.bytedance.com/)
[![Atlas Cloud](https://img.shields.io/badge/Run%20on-Atlas%20Cloud-orange)](https://www.atlascloud.ai?ref=JPM683)

**A curated collection of high-quality prompts, tips, and resources for ByteDance's Seedance 2.0 — the world's most advanced unified multimodal AI video generation model.**

CNN called it **"China's latest AI so powerful it's panicking Hollywood."**

[English](README.md) | [中文](README_zh-CN.md) | [日本語](README_ja.md) | [한국어](README_ko.md)

---

**If you find this useful, please star this repo!** Your support helps more creators discover these resources.

</div>

---

<div align="center">

### Run These Prompts Instantly on Atlas Cloud

The fastest and most affordable way to run Seedance 2.0 at full quality.

**Uncensored AI** | **Lowest Price from $0.222/video** | **2x Faster Inference**

[![Try Atlas Cloud](https://img.shields.io/badge/Try%20Atlas%20Cloud-Start%20Free-ff6b35?style=for-the-badge&logo=rocket&logoColor=white)](https://www.atlascloud.ai?ref=JPM683)

New users get **25% bonus** on first top-up (up to $100)

</div>

---

## Table of Contents

- [About Seedance 2.0](#about-seedance-20)
- [Quick Start (API)](#quick-start-api)
- [Prompt Collection](#prompt-collection)
  - [Ultra-Realistic Video Generation](#1-ultra-realistic-video-generation)
  - [Character & Scene Consistency](#2-character--scene-consistency)
  - [Advanced Camera Movements](#3-advanced-camera-movements)
  - [Creative Visual Effects](#4-creative-visual-effects)
  - [Story Development & Extension](#5-story-development--extension)
  - [Audio & Voice Synthesis](#6-audio--voice-synthesis)
- [Prompt Engineering Tips](#prompt-engineering-tips)
- [Official Resources](#official-resources)
- [Community Resources](#community-resources)
- [Pricing Comparison](#pricing-comparison)
- [FAQ](#faq)
- [Star History](#star-history)
- [Contributing](#contributing)
- [License](#license)

---

## About Seedance 2.0

**Seedance 2.0** is ByteDance's next-generation AI video generation model, released in **February 2026**. It is the first production-ready model to achieve **unified multimodal audio-visual joint generation** within a single architecture — producing cinematic video, synchronized audio, dialogue, music, and multi-shot narratives from a single prompt.

### Core Capabilities

| Capability | Details |
|:-----------|:--------|
| **Unified Audio-Visual Generation** | Single model produces video + synchronized audio + dialogue in one pass |
| **Complex Camera Movements** | Push-pull zoom, focus switching, tracking shots, POV switching, Hitchcock zoom, and more |
| **Multi-Shot Narrative** | Generate coherent multi-shot sequences maintaining character and scene consistency |
| **8+ Language Lip Sync** | Phoneme-level lip synchronization across 8+ languages including English, Chinese, Japanese, Korean |
| **Character Consistency** | Maintain consistent characters across shots using image/video references (`@image1`, `@video1`) |
| **Cinematic Quality** | Hollywood-grade visual quality with realistic lighting, depth of field, and motion blur |

### Key Specifications

| Spec | Value |
|:-----|:------|
| Max Resolution | Up to 1080p |
| Video Duration | 5s – 20s per generation |
| Aspect Ratios | 16:9, 9:16, 1:1, 4:3, 3:4 |
| Audio Channels | Stereo |
| Frame Rate | 24fps / 30fps |
| Input Modes | Text-to-Video, Image-to-Video, Video-to-Video |
| Reference Support | Multi-image (`@image1`, `@image2`), video reference (`@video1`) |

### Use Cases

- **Filmmaking & Pre-visualization** — Rapid storyboard-to-video, concept visualization, VFX previews
- **Advertising & Marketing** — Product commercials, brand campaigns, social media ads
- **Social Media & UGC** — Short-form content, TikTok/Reels, creative storytelling
- **E-commerce** — Product showcase videos, virtual try-on, lifestyle demos
- **Education & Training** — Explainer videos, historical recreations, scientific visualization
- **Music & Entertainment** — Music videos, lyric videos, concert visuals

---

## Quick Start (API)

Run Seedance 2.0 via Atlas Cloud's API in seconds. No GPU setup required.

### Get Your API Key

1. Sign up at [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683)
2. Navigate to **API Keys** in your dashboard
3. Create a new key and copy it

### cURL Example

```bash
# Use Atlas Cloud API to generate video with Seedance 2.0
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

### Python Example

```python
import requests
import time

# Atlas Cloud API configuration
API_KEY = "YOUR_API_KEY"
BASE_URL = "https://api.atlascloud.ai/api/v1/model"

def generate_video(prompt: str, duration: int = 10, aspect_ratio: str = "16:9"):
    """
    Call the Seedance 2.0 model to generate a video

    Parameters:
        prompt: Video generation prompt
        duration: Video duration (seconds)
        aspect_ratio: Video aspect ratio
    Returns:
        Result of the video generation task
    """
    # Submit video generation request
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
    print(f"Task submitted, ID: {task_id}")

    # Poll for generation status
    while True:
        status_resp = requests.get(
            f"{BASE_URL}/task/{task_id}",
            headers={"Authorization": f"Bearer {API_KEY}"}
        )
        status = status_resp.json()

        if status["status"] == "completed":
            print("Video generation complete!")
            return status["output"]["video_url"]
        elif status["status"] == "failed":
            raise Exception(f"Generation failed: {status.get('error')}")

        time.sleep(5)  # Check status every 5 seconds

# Usage example
video_url = generate_video(
    prompt="Camera slightly pulls back revealing the full street view and follows "
           "the female protagonist moving. The wind blows the hem of her dress as "
           "she walks on the streets of 19th century London. Cinematic lighting, "
           "film grain, anamorphic lens.",
    duration=15,
    aspect_ratio="16:9"
)
print(f"Video download URL: {video_url}")
```

### Response Handling

```json
{
  "task_id": "task_abc123",
  "status": "completed",
  "output": {
    "video_url": "https://cdn.atlascloud.ai/videos/task_abc123.mp4",
    "duration": 10,
    "resolution": "1920x1080",
    "audio_included": true
  },
  "usage": {
    "cost": 0.222,
    "model": "seedance-v1.5-pro"
  }
}
```

---

## Prompt Collection

> **How to use these prompts**: Copy any prompt below and paste it directly into the [Atlas Cloud playground](https://www.atlascloud.ai?ref=JPM683) or use the API. For prompts with `@image1` or `@video1` references, upload your reference image/video first.

---

### 1. Ultra-Realistic Video Generation

Prompts designed for photorealistic video output with natural motion and cinematic quality.

| # | Title | Difficulty | Duration | Aspect Ratio |
|:--|:------|:-----------|:---------|:-------------|
| 1.1 | Elegant Laundry Scene | Beginner | 10s | 16:9 |
| 1.2 | Interactive Painting Character | Intermediate | 10s | 9:16 |
| 1.3 | Victorian Street Scene | Intermediate | 15s | 16:9 |
| 1.4 | Chase Scene with Obstacles | Advanced | 15s | 16:9 |

<details>
<summary><b>1.1 Elegant Laundry Scene</b> — A serene domestic moment with natural physics</summary>

**Prompt:**
```
Fixed camera shot, a girl elegantly hanging clothes to dry, after finishing she takes out
another piece from the basket and shakes the clothes vigorously. The fabric flows naturally
in the breeze. Sunlight filters through the wet fabric creating beautiful light diffusion.
Warm afternoon lighting, shallow depth of field, 4K cinematic quality.
```

**Tips:**
- The "fixed camera" instruction keeps the shot stable and lets the subject's motion be the focus
- Mentioning "shakes the clothes vigorously" tests Seedance 2.0's physics simulation
- Adding light interaction details ("sunlight filters through") enhances realism

</details>

<details>
<summary><b>1.2 Interactive Painting Character</b> — Breaking the fourth wall with painted art</summary>

**Prompt:**
```
The character in the painting has a guilty expression, eyes looking left and right, then
peeks out of the frame, quickly extends their hand out of the frame to grab a cola and
takes a sip. After drinking, they let out a satisfied sigh, wipe their mouth, and retreat
back into the painting, resuming their original elegant pose as if nothing happened.
Oil painting style blending with photorealistic elements. Warm gallery lighting.
```

**Tips:**
- This prompt demonstrates Seedance 2.0's ability to blend artistic styles with realism
- The sequential actions (peek, grab, drink, retreat) test temporal coherence
- Perfect for social media content — highly shareable and engaging

</details>

<details>
<summary><b>1.3 Victorian Street Scene</b> — Period cinematography with tracking movement</summary>

**Prompt:**
```
Camera slightly pulls back (revealing the full street view) and follows the female
protagonist moving. The wind blows the hem of her dress as she walks on the streets
of 19th century London. Gas lamps flicker along cobblestone streets. Horse-drawn
carriages pass in the background. Pedestrians in period-appropriate attire populate
the scene. Fog rolls gently through the narrow lanes. Cinematic color grading with
desaturated tones, film grain, anamorphic lens flare. 4K resolution.
```

**Tips:**
- Camera pullback + tracking creates dynamic, professional cinematography
- Period-specific details (gas lamps, cobblestone, horse-drawn carriages) guide the model
- Mentioning "anamorphic lens flare" and "film grain" adds filmic quality

</details>

<details>
<summary><b>1.4 Chase Scene with Obstacles</b> — Fast-paced action with multiple characters</summary>

**Prompt:**
```
Camera follows a man in black clothes fleeing quickly through a crowded marketplace,
with a group of people chasing behind. He knocks over fruit stalls, ducks under hanging
fabrics, and leaps over a cart. The chasers stumble over the obstacles he leaves behind.
Handheld camera feel with slight shake. Fast-paced editing rhythm. Dramatic shadows and
high contrast lighting. Urban environment, daytime. Cinematic action movie style.
```

**Tips:**
- Multiple character interactions test the model's spatial reasoning
- Environmental destruction (knocking over stalls) adds dynamic complexity
- "Handheld camera feel" creates authentic action movie aesthetics

</details>

---

### 2. Character & Scene Consistency

Prompts utilizing reference images and videos (`@image1`, `@video1`) to maintain character identity and scene continuity across generations.

| # | Title | Reference Type | Difficulty | Duration |
|:--|:------|:---------------|:-----------|:---------|
| 2.1 | After-Work Homecoming | `@image1` | Intermediate | 10s |
| 2.2 | Opera Stage Transformation | `@video1` | Advanced | 15s |
| 2.3 | One-Take Seamless Transition | None (single prompt) | Advanced | 20s |
| 2.4 | Luxury Handbag Commercial | `@image1` + `@image2` | Intermediate | 10s |

<details>
<summary><b>2.1 After-Work Homecoming</b> — Consistent character from reference image</summary>

**Prompt:**
```
@image1 The woman in the reference image arrives home after a long day at work. She opens
the front door, drops her bag on the hallway table, kicks off her heels, and walks to the
kitchen. She opens the refrigerator, the cool light illuminates her tired but content face.
She grabs a bottle of water and takes a long sip. Warm interior lighting transitioning to
cool refrigerator light. Cinematic, intimate atmosphere. 16:9 aspect ratio.
```

**Tips:**
- `@image1` preserves the character's face, hair, and body proportions
- Sequential scene transitions (hallway → kitchen → refrigerator) test spatial consistency
- Lighting changes throughout the scene add production value

</details>

<details>
<summary><b>2.2 Opera Stage Transformation</b> — Video-referenced style transfer</summary>

**Prompt:**
```
@video1 Transform this performance into a grand Chinese opera stage setting. The performer
maintains the same movements and expressions from the reference video, but is now wearing
elaborate Peking opera costume with ornate headdress. The stage features traditional red
and gold decorations, dramatic theatrical lighting with colored spotlights. Smoke effects
drift across the stage floor. Traditional Chinese instrumental accompaniment plays in sync
with the movements. Cinematic wide shot gradually pushing in to medium close-up.
```

**Tips:**
- `@video1` preserves motion and timing from the reference video
- Style transfer from modern to traditional opera tests the model's creative range
- Audio generation is specified to match the visual transformation

</details>

<details>
<summary><b>2.3 One-Take Seamless Transition</b> — Complex continuous shot</summary>

**Prompt:**
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

**Tips:**
- This is an advanced prompt testing Seedance 2.0's spatial transition capabilities
- "No cuts" and "seamless" are key instructions for continuity
- Each environment has distinct lighting and atmosphere that must transition smoothly
- Recommended duration: 20 seconds for full effect

</details>

<details>
<summary><b>2.4 Luxury Handbag Commercial</b> — Product-focused with dual references</summary>

**Prompt:**
```
@image1 @image2 A luxury fashion commercial. The model from @image1 carries the handbag
from @image2. She walks confidently down a marble hallway in a grand European hotel.
Camera tracks alongside her at waist level, keeping the handbag in focus. She pauses at
a large window, golden hour light streams in, illuminating the bag's leather texture and
metallic hardware. She runs her fingers along the bag's stitching. Shallow depth of field,
the background softly blurs. Cut to a tabletop shot of the bag alone on a velvet surface
with dramatic side lighting. Premium commercial quality, 4K.
```

**Tips:**
- Dual reference (`@image1` for model, `@image2` for product) enables precise brand control
- Camera at waist level ensures the product stays prominently visible
- Golden hour + shallow DOF is a proven formula for luxury product videography

</details>

---

### 3. Advanced Camera Movements

Prompts showcasing Seedance 2.0's industry-leading camera control capabilities.

| # | Title | Camera Technique | Difficulty | Duration |
|:--|:------|:----------------|:-----------|:---------|
| 3.1 | Hitchcock Zoom in Elevator | Dolly zoom (vertigo effect) | Advanced | 10s |
| 3.2 | Complex Corridor Chase | Tracking + focus pull | Advanced | 15s |
| 3.3 | Car Commercial Cinematography | Orbital + crane + tracking | Expert | 15s |
| 3.4 | Martial Arts Combat Scene | Dynamic multi-angle | Advanced | 10s |

<details>
<summary><b>3.1 Hitchcock Zoom in Elevator</b> — The classic vertigo/dolly zoom effect</summary>

**Prompt:**
```
A man stands alone in a modern glass elevator ascending a tall building. As the elevator
rises, execute a Hitchcock dolly zoom effect — the camera physically moves backward while
zooming in, making the background stretch and distort while the man's size stays constant.
His expression shifts from calm to uneasy as the effect intensifies. The city skyline
visible through the glass walls appears to warp and stretch. Dramatic orchestral tension
builds. Cool blue-gray color grading, sharp focus on subject, background distortion.
Vertigo-inspired cinematography.
```

**Tips:**
- The dolly zoom (Hitchcock zoom / vertigo effect) is one of cinema's most powerful techniques
- Seedance 2.0 can simulate this complex optical phenomenon from text alone
- The emotional arc (calm → uneasy) should sync with the visual distortion

</details>

<details>
<summary><b>3.2 Complex Corridor Chase</b> — Multi-technique tracking shot</summary>

**Prompt:**
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

**Tips:**
- Multiple camera techniques in sequence: tilt, track, rack focus, whip pan, pullback
- Each transition should feel motivated by the action
- The "momentarily loses her" instruction adds realistic camera work

</details>

<details>
<summary><b>3.3 Car Commercial Cinematography</b> — Premium automotive videography</summary>

**Prompt:**
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

**Tips:**
- Multi-shot commercial with 5 distinct camera setups
- Each shot uses a different camera technique (orbital, tracking, crane, POV, aerial)
- Audio specification ("engine sound design") leverages unified audio-visual generation
- This prompt is best run at 15-20 seconds for the full sequence

</details>

<details>
<summary><b>3.4 Martial Arts Combat Scene</b> — Dynamic action cinematography</summary>

**Prompt:**
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

**Tips:**
- Speed variation (slow motion → real time → slow motion) creates dramatic rhythm
- "Camera weaves between the fighters" instructs intimate, immersive positioning
- The freeze-frame at impact is a signature action movie technique

</details>

---

### 4. Creative Visual Effects

Prompts exploring Seedance 2.0's ability to generate surreal, artistic, and effects-heavy content.

| # | Title | Style | Difficulty | Duration |
|:--|:------|:------|:-----------|:---------|
| 4.1 | VR Glasses Universe Journey | Sci-Fi / Surreal | Advanced | 15s |
| 4.2 | Fashion Quick-Change Commercial | Fashion / VFX | Intermediate | 10s |
| 4.3 | Ink Wash Tai Chi | Traditional Art / Motion | Intermediate | 15s |
| 4.4 | Magical Transformation Sequence | Fantasy / VFX | Advanced | 10s |
| 4.5 | Golden Particle Title Reveal | Motion Graphics / VFX | Intermediate | 8s |

<details>
<summary><b>4.1 VR Glasses Universe Journey</b> — Immersive sci-fi visualization</summary>

**Prompt:**
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

**Tips:**
- Scale transition from macro (glasses) to cosmic (space) and back tests Seedance 2.0's range
- Detailed environment descriptions at each scale ensure visual richness
- The "reflection in the lens" bookend creates a satisfying narrative loop

</details>

<details>
<summary><b>4.2 Fashion Quick-Change Commercial</b> — Rapid wardrobe transitions</summary>

**Prompt:**
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

**Tips:**
- Five distinct outfit changes test character consistency through transformations
- "Burst of fabric particles" gives the model a concrete visual transition to generate
- Music sync specification leverages the audio-visual joint generation

</details>

<details>
<summary><b>4.3 Ink Wash Tai Chi</b> — Traditional Chinese art in motion</summary>

**Prompt:**
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

**Tips:**
- Blending traditional art style with fluid animation is a signature Seedance 2.0 capability
- The "ink trails painting landscapes" adds creative visual complexity
- Specifying "guqin music" targets appropriate traditional Chinese instrumentation

</details>

<details>
<summary><b>4.4 Magical Transformation Sequence</b> — Fantasy metamorphosis</summary>

**Prompt:**
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

**Tips:**
- Sequential transformation gives the model clear temporal beats to follow
- Particle effects and energy visualization test VFX generation capabilities
- The emotional arc (ordinary → magical) is a proven storytelling framework

</details>

<details>
<summary><b>4.5 Golden Particle Title Reveal</b> — Motion graphics title sequence</summary>

**Prompt:**
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

**Tips:**
- Motion graphics prompts benefit from very specific timing and spatial descriptions
- The two-phase reveal (particles → solid) creates visual sophistication
- Audio sync ("bass impact on reveal") demonstrates audio-visual coordination

</details>

---

### 5. Story Development & Extension

Prompts for narrative-driven video content with clear story arcs.

| # | Title | Narrative Type | Difficulty | Duration |
|:--|:------|:---------------|:-----------|:---------|
| 5.1 | Comic Panel Animation | Sequential Narrative | Intermediate | 15s |
| 5.2 | Childhood Seasons Documentary | Documentary Montage | Advanced | 20s |
| 5.3 | Coffee Morning Campaign | Brand Story | Beginner | 10s |

<details>
<summary><b>5.1 Comic Panel Animation</b> — Bringing static panels to life</summary>

**Prompt:**
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

**Tips:**
- The comic panel → animation transition is highly engaging for social media
- Maintaining comic book visual style throughout tests artistic consistency
- Visual onomatopoeia ("WHOOSH") adds an authentic comic book element

</details>

<details>
<summary><b>5.2 Childhood Seasons Documentary</b> — Emotional time-lapse narrative</summary>

**Prompt:**
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

**Tips:**
- Aging the character across seasons tests Seedance 2.0's understanding of human development
- Each season has distinct color grading and atmosphere
- The dissolve transitions and piano melody create emotional continuity

</details>

<details>
<summary><b>5.3 Coffee Morning Campaign</b> — Brand storytelling commercial</summary>

**Prompt:**
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

**Tips:**
- ASMR-quality sound design leverages Seedance 2.0's audio generation for brand content
- The cool-to-warm color transition mirrors the narrative journey
- Macro close-ups of the coffee process create the sensory appeal brands want

</details>

---

### 6. Audio & Voice Synthesis

Prompts specifically designed to showcase Seedance 2.0's unified audio-visual generation capabilities, including dialogue, music, and sound effects.

| # | Title | Audio Feature | Difficulty | Duration |
|:--|:------|:-------------|:-----------|:---------|
| 6.1 | Cat & Dog Roast Battle | Character Dialogue | Advanced | 15s |
| 6.2 | Chinese Opera Performance | Musical Vocal | Advanced | 15s |
| 6.3 | Cinematic Road Trip MV | Music + Visuals | Expert | 20s |

<details>
<summary><b>6.1 Cat & Dog Roast Battle</b> — Comedic character dialogue with lip sync</summary>

**Prompt:**
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

**Tips:**
- Phoneme-level lip sync on animal characters is a signature Seedance 2.0 feat
- Distinct voice characterization (sassy cat vs. dopey dog) tests voice synthesis range
- The reality TV format is highly shareable on social media platforms

</details>

<details>
<summary><b>6.2 Chinese Opera Performance</b> — Traditional vocal + visual art</summary>

**Prompt:**
```
A Peking opera performer in full traditional costume and elaborate face paint (jing role,
painted face) stands center stage. Dramatic red and gold stage lighting. He begins
performing a classic aria — his voice carries the distinctive high-pitched, powerful
vibrato of Peking opera singing. The camera starts on a medium shot and slowly pushes
in to a close-up during the emotional peak of the aria. His painted expressions are
visible in detail — each gesture precise and traditional. Sleeve water sleeves (水袖)
flow with his arm movements. The traditional percussion and string ensemble accompanies
his vocal. As the aria reaches its climax, the camera rotates around him in a slow
360-degree orbit. Stage smoke drifts at floor level. Dramatic theatrical lighting shifts
from warm gold to intense red at the climax. Authentic Peking opera vocal quality and
instrumentation.
```

**Tips:**
- Peking opera vocal synthesis demonstrates the model's cultural audio capabilities
- Specific costume and performance terminology helps generate authentic visuals
- The 360-degree orbit shot adds cinematic flair to traditional performance

</details>

<details>
<summary><b>6.3 Cinematic Road Trip MV</b> — Music video with synchronized audio</summary>

**Prompt:**
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

**Tips:**
- Music generation + visual sync is the pinnacle of Seedance 2.0's unified model
- Beat-synced editing instructions ("rapid montage cut to the beat") guide temporal rhythm
- Each scene has specific emotional tone matching the musical structure

</details>

---

## Prompt Engineering Tips

Master these techniques to get the most out of Seedance 2.0.

### Camera Movement Keywords

| Keyword | Effect | Best For |
|:--------|:-------|:---------|
| `Fixed camera` | Static shot, no movement | Dialogue scenes, product shots |
| `Camera tracks` / `Tracking shot` | Camera follows subject laterally | Walking scenes, chases |
| `Camera pushes in` / `Push-in` | Forward dolly movement | Building tension, reveals |
| `Camera pulls back` / `Pullback` | Backward dolly movement | Reveals, establishing shots |
| `Dolly zoom` / `Hitchcock zoom` | Zoom + counter-dolly | Psychological tension |
| `Orbital shot` / `Camera orbits` | 360-degree rotation around subject | Product showcases, hero shots |
| `Crane shot` | Vertical ascending/descending | Grand reveals, scene openings |
| `Whip pan` | Rapid horizontal pan | Transitions, action scenes |
| `Rack focus` / `Focus pull` | Shift focus between planes | Directing attention, transitions |
| `POV shot` / `First-person` | Subject's perspective | Immersive experiences |
| `Aerial` / `Drone shot` | High-altitude overhead | Landscapes, establishing shots |
| `Low angle` | Camera below eye level | Making subjects appear powerful |
| `Dutch angle` / `Canted angle` | Tilted frame | Tension, disorientation |

### Audio & Voice Control

> **Key insight:** Seedance 2.0 generates audio as part of the same model pass — not as a separate post-processing step. This means audio-visual synchronization is inherently precise.

| Technique | Example Prompt Fragment |
|:----------|:----------------------|
| **Character dialogue** | `He says in a deep voice: "The time has come."` |
| **Sound effects** | `The sound of thunder rolls across the valley` |
| **Music style** | `Upbeat jazz piano plays in the background` |
| **Ambient audio** | `Birds chirping, leaves rustling, distant waterfall` |
| **Vocal singing** | `She sings a soft lullaby in a warm soprano voice` |
| **Lip sync language** | `She speaks in Japanese: "はじめまして"` |
| **Audio transition** | `The busy street noise fades to peaceful silence` |
| **No audio** | `Silent. No sound. Muted.` |

### Multi-Reference Techniques

```
# Single character reference
@image1 The person from the reference walks into a café...

# Multi-reference combination (character + product)
@image1 @image2 The model from @image1 holds the product from @image2...

# Video reference (maintain motion)
@video1 Recreate the movements from the reference video in a new setting...

# Multi-character consistency
@image1 @image2 @image3 Three friends from the reference images meet at a park...
```

### Duration Optimization Guide

| Content Type | Recommended Duration | Why |
|:-------------|:--------------------|:----|
| Product shot | 5–8s | Short, focused, repeatable |
| Social media clip | 8–10s | Optimal for Reels/TikTok attention span |
| Narrative scene | 10–15s | Enough for a mini story arc |
| Complex multi-shot | 15–20s | Room for 3–5 distinct shots |
| Music video segment | 15–20s | Full verse or chorus |

### Aspect Ratio Guide

| Ratio | Resolution | Best For |
|:------|:-----------|:---------|
| **16:9** | 1920x1080 | YouTube, cinematic, landscape |
| **9:16** | 1080x1920 | TikTok, Reels, Stories |
| **1:1** | 1080x1080 | Instagram feed, thumbnails |
| **4:3** | 1440x1080 | Vintage film look, presentations |
| **3:4** | 1080x1440 | Portrait photography style |

---

## Official Resources

| Resource | Link | Description |
|:---------|:-----|:------------|
| ByteDance Seed | [seed.bytedance.com](https://seed.bytedance.com/) | Official Seed model family homepage |
| Jimeng AI | [jimeng.jianying.com](https://jimeng.jianying.com/) | Official Chinese platform for Seedance |
| Seedance Research Paper | [arxiv.org](https://arxiv.org/) | Technical paper on unified audio-visual generation |
| ByteDance Research | [research.bytedance.com](https://research.bytedance.com/) | ByteDance AI research portal |
| Seed Video Blog | [bytedance.com/blog](https://bytedance.com/) | Official blog posts and announcements |

---

## Community Resources

### Tools & Integrations

| Tool | Description | Link |
|:-----|:------------|:-----|
| **ComfyUI-Seedance** | ComfyUI nodes for Seedance integration | Community GitHub |
| **Seedance Prompt Builder** | Web-based visual prompt builder | Community tool |
| **Atlas Cloud Playground** | Web UI for running Seedance with no code | [atlascloud.ai](https://www.atlascloud.ai?ref=JPM683) |

### Tutorial Videos

- **Getting Started with Seedance 2.0** — Basic prompt writing and generation workflow
- **Advanced Camera Techniques in Seedance** — Mastering complex camera movements
- **Seedance Audio-Visual Sync** — Leveraging unified audio-video generation
- **Character Consistency Masterclass** — Using image references for consistent characters
- **Commercial Production with Seedance** — Creating professional advertising content

### Community Forums

- Reddit: r/seedance, r/aivideo
- Discord: Seedance Community Server
- X/Twitter: #Seedance2 #SeedancePrompts

---

## Pricing Comparison

Choose the best platform to run your Seedance prompts.

| Provider | Price / Video | Speed | Quality | NSFW | API Access | Audio Included |
|:---------|:-------------|:------|:--------|:-----|:-----------|:---------------|
| **Atlas Cloud** | **$0.222** | Fast | Top | Yes | Yes | Yes |
| Jimeng (Official) | Limited free | Medium | Top | No | Limited | Yes |
| Other Providers | $0.30+ | Varies | Varies | No | Varies | Varies |

### Atlas Cloud Pricing Details

| Model | Type | Price | Speed |
|:------|:-----|:------|:------|
| Seedance v1.5 Pro | Text-to-Video | $0.222 / request | Standard |
| Seedance v1.5 Pro | Image-to-Video | $0.222 / request | Standard |
| Seedance v1.5 Pro Fast | Text-to-Video | Lower | 2x Faster |
| Seedance v1.5 Pro Fast | Image-to-Video | Lower | 2x Faster |
| Seedance v1 Lite | Text-to-Video | Budget | Standard |

> **90% discount** currently available on Atlas Cloud. Prices shown are after discount.

---

## FAQ

<details>
<summary><b>What is Seedance 2.0?</b></summary>

Seedance 2.0 is ByteDance's state-of-the-art AI video generation model released in February 2026. It is the first production model to achieve unified multimodal audio-visual joint generation — meaning a single model generates cinematic video, synchronized audio, dialogue, music, and multi-shot narratives from text prompts. CNN described it as "China's latest AI so powerful it's panicking Hollywood."

</details>

<details>
<summary><b>How is Seedance 2.0 different from other AI video models?</b></summary>

Seedance 2.0's key differentiator is its **unified multimodal generation**. Unlike competitors that generate video and audio separately, Seedance 2.0 produces both in a single model pass, ensuring perfect synchronization. It also supports complex camera movements (dolly zoom, tracking, POV switching), 8+ language phoneme-level lip sync, and multi-shot narrative coherence — capabilities that most competitors lack.

</details>

<details>
<summary><b>What is the cheapest way to run Seedance 2.0?</b></summary>

The most cost-effective way to run Seedance 2.0 is through [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683) at **$0.222 per video** (90% discount currently active). New users also receive a **25% bonus on their first top-up** (up to $100 bonus). This is significantly cheaper than other API providers which typically charge $0.30 or more per generation.

</details>

<details>
<summary><b>Can Seedance 2.0 generate audio and dialogue?</b></summary>

Yes. Seedance 2.0 features unified audio-visual generation. You can specify dialogue (with lip sync in 8+ languages), background music, sound effects, and ambient audio directly in your prompt. The model generates synchronized audio as part of the same generation pass — not as a separate post-processing step.

</details>

<details>
<summary><b>What resolutions and durations does Seedance 2.0 support?</b></summary>

Seedance 2.0 supports resolutions up to 1080p in multiple aspect ratios (16:9, 9:16, 1:1, 4:3, 3:4). Video duration ranges from 5 to 20 seconds per generation. Frame rates of 24fps and 30fps are supported.

</details>

<details>
<summary><b>How do I maintain character consistency across multiple videos?</b></summary>

Use the reference system: upload a character image and reference it with `@image1` in your prompt. For example: `@image1 The person from the reference walks into a café...` This preserves facial features, body proportions, and key visual characteristics. You can also use `@video1` to reference motion and timing from a previous generation.

</details>

<details>
<summary><b>What languages does Seedance 2.0 support for lip sync?</b></summary>

Seedance 2.0 supports phoneme-level lip synchronization in 8+ languages, including English, Chinese (Mandarin), Japanese, Korean, French, Spanish, German, and more. Simply write dialogue in the target language within your prompt, and the model will generate matching lip movements.

</details>

<details>
<summary><b>Can I use Seedance 2.0 for commercial projects?</b></summary>

Yes. When accessed through platforms like Atlas Cloud, the generated content can be used for commercial purposes including advertising, social media marketing, product videos, and more. Always check the specific terms of service for the platform you use.

</details>

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=atlascloud/awesome-seedance-2-prompts&type=Date)](https://star-history.com/#atlascloud/awesome-seedance-2-prompts&Date)

---

## Bring Your Creative Vision to Life

Love these prompts? Run them instantly on **Atlas Cloud** — the industry's most cost-effective AI platform with full creative freedom.

| Benefit | Details |
|:--------|:--------|
| **Uncensored AI** | 100% creative freedom, no content restrictions |
| **Lowest Price** | Starting from $0.222/video with 90% discount |
| **High Performance** | Fast inference, no queue wait times |
| **25% Bonus** | New users get up to $100 bonus on first top-up |
| **Full API Access** | REST API, Python SDK, and web playground |

<div align="center">

[![Start Generating on Atlas Cloud](https://img.shields.io/badge/Start%20Generating%20on%20Atlas%20Cloud-ff6b35?style=for-the-badge&logo=rocket&logoColor=white)](https://www.atlascloud.ai?ref=JPM683)

**Friends get 25% bonus on first recharge (max $100)**

</div>

---

## Contributing

Contributions are welcome! If you have great Seedance 2.0 prompts, tips, or resources to share:

1. **Fork** this repository
2. **Create** a new branch (`git checkout -b feature/my-awesome-prompt`)
3. **Add** your content following the existing format
4. **Submit** a Pull Request with a clear description

### Contribution Guidelines

- Prompts must be **tested and verified** to produce good results with Seedance 2.0
- Include **difficulty level** and **recommended duration** for each prompt
- Provide **tips** explaining why the prompt works
- Follow the existing table and formatting structure
- Update all language versions (EN, ZH-CN, JA, KO) if possible

---

## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

<div align="center">

**Made with passion for the AI video generation community**

If this repo helped you, please give it a star and share it with fellow creators!

[Report Bug](https://github.com/atlascloud/awesome-seedance-2-prompts/issues) | [Request Prompt](https://github.com/atlascloud/awesome-seedance-2-prompts/issues) | [Contribute](https://github.com/atlascloud/awesome-seedance-2-prompts/pulls)

</div>
