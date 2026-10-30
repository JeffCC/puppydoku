# 🐶 Puppydoku 皇后謎題 / Queens Puzzle

網頁版的 Puppydoku 謎題，融合數獨與「八皇后問題」的邏輯。

A web-based Puppydoku puzzle that blends Sudoku with the logic of the N-Queens problem.

**線上遊玩 / Play online: https://jeffcc.github.io/puppydoku/**

也可以直接用瀏覽器開啟 `index.html`，不需安裝任何東西。網頁會依瀏覽器語系自動切換中英文（zh=中文，其他=英文）。

You can also just open `index.html` in a browser — nothing to install. The page auto-switches between Chinese and English based on the browser's locale (zh = Chinese, others = English).

訪客統計使用 GoatCounter（只在 GitHub Pages 上啟用），代碼設定在 `index.html` 開頭的 `GOATCOUNTER`。

Visitor stats use GoatCounter (only enabled on GitHub Pages). The account code is set in `GOATCOUNTER` at the top of `index.html`.

## 規則 / Rules

1. 小狗不能相鄰：上下、左右、斜角（周圍 8 格）都不能有其他小狗
2. 每一橫列剛好 1 隻
3. 每一直行剛好 1 隻
4. 每個顏色區域剛好 1 隻

---

1. Puppies can't be adjacent — none of the 8 surrounding cells (orthogonal + diagonal) may hold another puppy
2. Exactly 1 puppy per row
3. Exactly 1 puppy per column
4. Exactly 1 puppy per color region

## 功能 / Features

- 自動出題：5×5 到 11×11，每題都驗證為唯一解
- 一鍵排除：選取小狗後按 `E`，把同橫列、同直行、周圍 8 格（可選同色區域）標成 ✖；`A` 對全部小狗排除
- 推理提示：顯示下一步的推理過程（藍框為依據、橘框為結論），可一鍵套用
- 衝突與死路提示、復原、計時
- 自動完成：放好倒數第二隻小狗後，若盤面只剩最後一格空格且正是小狗，自動放好並停止計時
- 標記模式切換（✕ / 🐶 / ？，手機與電腦皆可用）；手機防止連點兩下放大畫面
- 中英文介面依瀏覽器語系自動切換

---

- Auto-generated puzzles from 5×5 to 11×11, each verified to have a unique solution
- One-click exclude: with a puppy selected, press `E` to mark ✖ on same row, same column, surrounding 8 cells (and optionally the same-color region); `A` excludes around all puppies
- Reasoning hints: shows the next reasoning step (blue = premise, orange = conclusion), with one-click apply
- Conflict and dead-end indicators, undo, timer
- Auto-finish: after placing the second-to-last puppy, if only one empty cell remains and it's exactly the last puppy, it's placed automatically and the timer stops
- Mark-mode switcher (✕ / 🐶 / ？, works on both mobile and desktop); mobile double-tap-zoom prevention
- UI auto-switches between Chinese and English based on browser locale

## 操作 / Controls

| 操作 | 效果 |
|---|---|
| 棋盤上方 ✕ / 🐶 / ？ 小圖示（或 `1` / `2` / `3`） | 選擇點一下要放的標記 |
| 點一下 | 放目前模式的標記（再點一次取消） |
| 拖曳 | 把經過的空白格標成 ✖ |
| 右鍵 / 長按 | 放「另一種」：✕、？ 模式放 🐶；🐶 模式放 ✕ |
| ？ 模式 | 標記不確定的格子；按 🐶 全部 ？ 變小狗，再按一次 ？（或 ✕）全部清除 |
| 方向鍵 / `Space` / `D` / `X` / `?` | 移動選取 / 循環切換 / 小狗 / 叉叉 / 不確定 |
| `E` / `A` | 排除選取小狗周圍 / 全部小狗排除 |
| `Ctrl+Z` | 復原 |

---

| Action | Effect |
|---|---|
| ✕ / 🐶 / ？ icons above the board (or `1` / `2` / `3`) | Choose which mark a tap places |
| Tap | Place the current mode's mark (tap again to clear) |
| Drag | Mark every empty cell dragged over with ✖ |
| Right-click / long-press | Place the "other" mark: ✕ / ？ modes place 🐶; 🐶 mode places ✕ |
| ？ mode | Mark uncertain cells; tap 🐶 to turn all ？ into puppies, tap ？ (or ✕) again to clear all ？ |
| Arrows / `Space` / `D` / `X` / `?` | Move selection / cycle / puppy / cross / uncertain |
| `E` / `A` | Exclude around selected puppy / exclude around all puppies |
| `Ctrl+Z` | Undo |
