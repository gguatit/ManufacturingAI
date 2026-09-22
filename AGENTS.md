# AGENTS.md

Docs root (`isa-95.html`) is build-free. Build/test/lint only inside `실습/`.

- Root: public git repo (`gguatit/ManufacturingAI` on GitHub). No package manager/build/test/lint. Do not scaffold anything next to `isa-95.html`.
- `실습/` is the only workspace: create venvs, install packages, run builds/tests, and write scratch files there.
- `제조AI-교재/`: course outputs. `제조AI-교재-단일.md` (옵시디언 전문, 이미지 내장), `제조AI-요약.md`, `스터디/` (16개 영역별 학습 파일), `용어정리/` (용어 해설 39개), `제조AI-교재-웹.html`, `원본자료/` (원본 docx + 이미지).
- This folder is an Obsidian vault (`.obsidian`): notes link by `[[파일명]]`, so renaming a note file breaks links — update every `[[...]]` reference in the same change.
- `isa-95.html` stays fully self-contained (inline CSS, no external deps): no CDN links, no separate CSS/JS files.
- Preview docs with `Start-Process "isa-95.html"` (workdir: this folder). No dev server needed.
- Content conventions for docs: Korean prose, no emoji, monochrome/grayscale palette only, print-friendly (`Ctrl+P` must still work).
- Paths contain spaces and Korean characters. Always quote with `-LiteralPath "..."` in PowerShell; never `cd`, use `workdir` param instead.
