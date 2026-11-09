# Paintcress 1.0 TEST
Native Android Paint Area whole-room shading deduction puzzle. Android 8+ (min26), target35. Package com.gg007.paintcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Paint Area deduction on a 4x4 grid. Shade or clear whole outlined rooms by tapping any of their cells. Each number counts dark cells sharing an edge with that cell, not dark rooms. Count each neighboring cell separately, even if several belong to the same room. Numbered cells may be dark or light. All dark cells must form one side-connected network. No 2x2 block may be entirely dark or entirely light. Light cells need not connect. Twelve original room layouts and unique shadings, automatic checking, unlimited whole-room undo/reset, next and level selection. Saved palette and optional dark cell marks. No timer, score or drag controls.

## Download and status
https://mega.co.nz/#!MVMTxbAb!cIRd6zg4Q3_uaG4hiLBtEK70RQSyT1B3TTPejAh2Mbg
APK SHA256 b1a44f3fe738fd301aaa8eaf5bc3dd9e5b00496f68c28e0d82aae0e70685d191; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent coordinate-neighbor lists, room-color maps and queue connectivity versus production mask counts and flood checks passed 786,432 complete board masks and 65,536 shape masks. Each of twelve original 4x4 room-and-clue boards has exactly one shading, and all twelve shadings differ. Tests cover whole-room toggles, numbered rooms changing color, separate dark groups, both solid-square colors, bounds, undo, reset and solved lock. Portable generator seed 530509 reproduces twelve distinct seven-room boards in 83 attempts. Actual drawing-adapter taps solve all twelve boards; solve/undo/replay, next, levels, menu, privacy and saved palette/dark marks pass. Six drawing previews inspected, not phone screenshots. Thin cell guides were added after the first visual inspection and the signed build and adapter tests rerun. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 184 prior studio descriptions and targeted functional terms across 803 web registry records. Mossmaze shares whole-room shading and both-color 2x2 bans, but solves a light tree maze with S-to-G and circle constraints. Paintcress instead counts local dark neighboring cells at clues, allows numbered rooms to darken, and connects the dark network; it does not require a light tree or light connectivity. Dualfern connects both colors with individual-cell toggles; Paintcress couples whole rooms and uses local counts with dark-only connectivity. No Paint Area match found in the reviewed corpus; repository corpus remains partial. Known Paint Area adaptation, not a global invention claim. Original generated boards, code and visuals, no copied puzzle layouts, code or art.
Rules https://www.nikoli.co.jp/ja/puzzles/paint_area/ ; independent rules https://www.janko.at/Raetsel/Peintoeria/index.htm .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/paintcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.paintcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Paintcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, dark cell marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 185-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/jzobz01fnh9h-paintcress-source-archive . Repository https://github.com/iLanis-agent/paintcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
