# Verification record

Tested October 10, 2026 in Microsoft Edge using browser automation, served from a local HTTP server.

Passed:
- JavaScript syntax checks.
- All 18 exhibit popups open and close.
- All six room challenges: visit requirements, incorrect-answer feedback, correct answers, and passport stamps.
- Timeline ordering and feedback; source detective scoring and explanations.
- Reflection saving, passport persistence, 22 bibliography/assignment entries.
- Video configuration download and rejection of unsafe or unsupported URL input.
- A real, short, locally generated WebM played to its natural end and automatically unlocked the museum.
- Missing video triggered a recovery entrance.
- Desktop visual review at 1440 pixels; mobile visual review and no horizontal page overflow at 390 pixels.
- Escape closes exhibit dialogs. No application JavaScript errors during the main interaction checks.

Limits:
- No user introductory video has been provided. YouTube live playback, embedding permissions, captions, school-network filtering, and the student's eventual video require testing with the final media.
- Archival audio/video is provided through credited archive links; those remote players and the remotely hosted photograph can change or be blocked.
- Hosting instructions were checked against GitHub and Vercel documentation, but the project has not been uploaded or deployed to an account.
- The video entrance is a self-guided learning flow, not a tamper-proof viewing requirement. Browser controls permit seeking, and a labeled recovery path is available.
