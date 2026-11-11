# nikke-api-media

[nikke-api](https://github.com/leegunwoooo/nikke-api)용 미리 렌더된 캐릭터 애니메이션.

| 디렉터리 | 내용 | 파일명 |
|---|---|---|
| `spine-gif/` | 로비(stand) idle 애니메이션 GIF — 384×384, 20fps, 투명 배경 | `<resourceId>_<skinIndex>.gif` (skinIndex 0 = 기본 외형) |

jsDelivr 경유로 서빙됩니다:

```
https://cdn.jsdelivr.net/gh/leegunwoooo/nikke-api-media@main/spine-gif/10_0.gif
```

API에서는 `/api/nikkes/:id/spine` 응답의 `stand.gif` 필드와
`/api/nikkes/:id/spine.gif?skin=` 리다이렉트로 노출됩니다.

생성: `nikke-api` 저장소의 `scripts/render-spine-gifs.ts`
(Spine 4.1 canvas 런타임으로 직접 렌더 — 스켈레톤/텍스처 원본 에셋은 여기 포함하지 않음).

© SHIFT UP / Level Infinite — 비공식 팬 데이터입니다.
