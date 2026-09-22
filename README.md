# 보송이

<img src="bosongi-preview.png" alt="보송이 기본 모습" width="180">

사과를 좋아하는 호기심 많은 레서판다, 보송이의 Codex v2 커스텀 펫 패키지입니다.

## 포함 파일

- `pet.json`: 펫 이름, 설명, 스프라이트 버전, 이미지 경로를 정의합니다.
- `spritesheet-20260917n.webp`: 현재 적용 중인 8×11 v2 스프라이트 시트입니다.
- `BOSONGI_STYLE_GUIDE.md`: 이후 수정 시 지켜야 할 색상, 형태, 모션 기준입니다.

## 설치

아래 파일을 Codex 펫 폴더에 함께 둡니다.

```text
~/.codex/pets/bosongi/
├── pet.json
├── spritesheet-20260917n.webp
└── BOSONGI_STYLE_GUIDE.md
```

`pet.json`의 `spritesheetPath`는 이미지 파일명과 같아야 합니다.

## 모션 구성

| 행 | 상태 | 프레임 |
| --- | --- | ---: |
| 0 | idle | 6 |
| 1 | running-right | 8 |
| 2 | running-left | 8 |
| 3 | waving | 4 |
| 4 | jumping / 사과 먹기 | 5 |
| 5 | failed | 8 |
| 6 | waiting | 6 |
| 7 | active work / 맥북 타이핑 | 6 |
| 8 | review / 맥북 타이핑 | 6 |
| 9–10 | 포인터 바라보기 16방향 | 16 |

idle은 고개와 시선을 부드럽게 좌우로 움직이며 윙크와 눈웃음으로 이어집니다. waiting은 두 손을 모은 기대 자세로 사용자 입력을 기다립니다. 좌우 running은 대각 측면에서 옆태로 이어지는 8단계 보행 주기입니다.

## 스프라이트 규격

- 버전: `spriteVersionNumber: 2`
- 크기: 1536×2288 px
- 그리드: 8열 × 11행
- 셀 크기: 192×208 px
- 배경: 투명

## 현재 버전

`20260917n`
