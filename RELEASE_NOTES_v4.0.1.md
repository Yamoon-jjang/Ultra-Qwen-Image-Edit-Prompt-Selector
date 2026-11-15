# v4.0.1 — 검색 결과를 현재 이미지 수로 / Search scoped to your image count

## 한국어

프리셋 검색을 더 정확하고 안전하게 다듬은 유지보수 릴리스입니다.

### 🔍 검색이 이제 선택한 이미지 수를 따릅니다
- **고친 문제:** "의상"처럼 검색하면 선택한 이미지 수(1·2·3장)와 상관없이 모든 결과가 섞여 나왔습니다.
- **지금:** 기본적으로 **현재 이미지 수의 프리셋만** 검색 결과에 나옵니다. 예: 2장을 고른 상태에서 "의상" → 2장 프리셋 66개만 표시.
- 검색 중 **편집 이미지 수 1·2·3 버튼**을 누르면 검색어는 그대로 두고 결과만 바뀝니다.

### ➕ ‘다른 이미지 수도 보기’ 토글 (새 기능)
- 검색어를 입력하면 결과 개수 줄 오른쪽에 버튼이 나타납니다. **기본값은 꺼짐**입니다.
- 켜면 1·2·3장 프리셋 전체에서 찾고, `1개 46 · 2개 66 · 3개 56`처럼 이미지 수별 개수를 보여줍니다.
- **현재 선택한 이미지 수의 결과가 맨 앞**에 오고, 나머지가 그 뒤에 이어집니다.
- 현재 이미지 수에 결과가 없으면 안내 문구가 이 토글을 알려줍니다.

### 🛡️ 선택 항목이 갑자기 사라지던 문제 수정
- **고친 문제:** 검색 결과에서 다른 이미지 수 프리셋을 누르면, 이미 골라 둔 항목이 **경고 없이 모두 지워졌습니다**. 매뉴얼에는 확인 창이 뜬다고 되어 있었지만 실제로는 없었습니다.
- **지금:** 선택한 항목이 있으면 확인 창이 먼저 뜨고, **‘취소’를 누르면 아무것도 바뀌지 않습니다.** 선택한 항목이 없으면 확인 없이 바로 전환됩니다.

### 📘 매뉴얼
- 한글·영문 매뉴얼의 검색 설명, 문제 해결, Q&A를 실제 동작에 맞게 고쳤습니다.

### ✅ 점검
- 검색이 아닐 때의 프리셋 목록(1·2·3장, NSFW), 프롬프트 생성 결과, 커스텀 항목 추가·검색, 카테고리 필터, KO/EN 전환이 v4.0.0과 똑같이 동작하는지 브라우저에서 확인했습니다.

**설치·업데이트:** 첨부 ZIP을 풀고 `Ultra_qwen_prompt_selecter_v4.html`을 Chrome 또는 Edge로 여세요. 파일 이름은 그대로이므로 기존 파일을 바꿔 넣으면 됩니다.
> 💡 **영구 저장으로 HTML 파일 안에 커스텀 프리셋을 넣어 두셨다면,** 새 HTML 파일을 연 뒤 다시 영구 저장해야 커스텀 프리셋이 유지됩니다. 브라우저에 저장된 커스텀 프리셋은 그대로 불러옵니다. 바꾸기 전에 기존 HTML 파일을 백업해 두세요.

## English

A maintenance release that makes preset search more accurate and safer.

### 🔍 Search now follows your image count
- **Fixed:** A search such as "outfit" showed every match regardless of the selected image count (1, 2 or 3 images).
- **Now:** Search shows **only presets for the current image count** by default.
- While searching, the **Input Images 1/2/3** buttons keep your search text and switch the results.

### ➕ New “Show other image counts” toggle
- Appears next to the result count while a search is active. **Off by default.**
- When on, results from all three image-count libraries are shown with a per-count breakdown.
- **Results for your current image count are listed first.**
- If the current count has no matches, the empty-result message points to this toggle.

### 🛡️ No more silently cleared selections
- **Fixed:** Picking a search result for a different image count **cleared your selected presets without warning** (the manual described a confirmation that did not exist).
- **Now:** If you have selections, the app asks first — **Cancel keeps everything unchanged.** With nothing selected, it switches immediately.

### 📘 Manuals
- Search, troubleshooting and FAQ sections of the Korean and English manuals now match the app.

### ✅ Verified
- Non-search preset lists (1/2/3 images, NSFW), prompt output, custom preset add/search, category filters and KO/EN switching were checked in a browser to behave exactly as in v4.0.0.

**Install / update:** Extract the attached ZIP and open `Ultra_qwen_prompt_selecter_v4.html` in Chrome or Edge. The filename is unchanged, so you can simply replace your old copy.
> 💡 **If you embedded custom presets with Permanent Save,** open the new HTML file and run Permanent Save again to keep them in the file. Presets stored in your browser load automatically. Back up your old HTML file first.
