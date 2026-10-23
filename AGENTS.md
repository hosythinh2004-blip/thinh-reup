# Coding agent instructions — Thinh Video Studio

- Never claim a Windows .exe was built or verified unless logs/artifacts prove it.
- Prioritize video-to-video workflow, synchronized narration, subtitle replacement, and preserving background audio.
- Run tests after each change; report passed, failed, and skipped tests separately.
- Check GPU support by actual encoding/inference tests rather than GPU-name or encoder-name detection.
- Do not introduce product activation locks, hidden credential collection, or Chrome cookie extraction.
- Use only officially supported AI account/API authorization and obey provider usage limits.
- Do not commit secrets, browser profiles, media from users, or large pretrained model weights.
- Work through feature branches and PRs; never overwrite unrelated repositories.
