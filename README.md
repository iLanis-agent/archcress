# Archcress 1.0 TEST
Native Android Akiperago island-shading puzzle. Android 8+ (min26), target35. Package com.gg007.archcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Akiperago (Archipelago) on a 4x4 grid. Shade land into islands joined by edges. Islands that touch at corners, directly or through a chain, form an archipelago. Every island must belong to an archipelago of at least two islands. A group with N islands must contain exactly one island of each area 1 through N. Order and shape do not matter. Gold numbered cells stay land; each number gives the full area of its own island. An island may contain no clue or multiple equal clues. Separate archipelagos satisfy the size rule independently. Sea has no connectivity or 2x2 restriction. Tap unnumbered cells to shade or clear land. Undo/reset, levels and next; saved palette and optional land marks. No timer or score.

## Download and status
https://mega.co.nz/#!kc1hwRTD!KDpqOECQTDIT78707fOorfBp97TUWy5-_VfA7hm8A08
APK SHA256 e23defa1bdb6857295108ca18288c9a5b335c51dc7de22c26a0a8bd92c402f80; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Production bit floods and union-find corner grouping agree with an independent coordinate adjacency BFS oracle on all 65,536 shadings of the 4x4 grid: exactly 404 are legal without clues. All 786,432 board/candidate checks agree. The portable seed-651109 generator enumerates every shading, selects legal islands and removes number clues only while one solution remains. Twelve original clue boards each have exactly one solution and all twelve shadings differ. Island areas, corner transitivity, complete size sets, singleton rejection, fixed clue locks, bounds, toggle/clear, undo/reset, solved lock and malformed states pass. Actual drawing-adapter taps solve all twelve and check undo/replay, next, levels, menu, privacy and saved palette/land marks. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 196 prior live studio descriptions and byte-current 803 web registry entries using functional terms. No Akiperago/Archipelago size-sequence match in this partial corpus. Shapechain enforces different shapes within corner chains; Diagonara uses individual size clues and a connected white sea without 2x2; Reefhaven has edge-separated numbered white islands in one sea. Archcress instead groups edge-connected dark islands by corner contact and requires each group to have every area from 1 to its island count exactly once. Its sea is unrestricted. Known Akiperago adaptation with original generated boards, code and visuals; no copied layouts/code/art or global invention claim. Six fetched rule pages from four sites agree on core rules. No history claim.
Rules https://www.janko.at/Raetsel/Akiperago/index.htm ; independent rules https://www.cross-plus-a.com/html/cros7aprg.htm .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/archcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.archcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Archcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, land marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 197-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/ykc53ccoqd19-archcress-source-archive . Repository https://github.com/iLanis-agent/archcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
