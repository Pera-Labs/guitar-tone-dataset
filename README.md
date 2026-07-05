# Guitar Tone Dataset

An open dataset of **researched guitar tones for 800+ famous songs** — the original gear (guitar, amp, pedals) and starting amp settings (gain, bass, mid, treble, presence, reverb) behind iconic riffs, with source citations.

Maintained by **[GuitarToneAdapt](https://guitartoneadapt.com)** — a free web app that re-dials any famous song's guitar tone for the specific guitar, amp and pedals *you* own.

## What's in it

`guitar-tones.json` — an array of tone entries. Each entry:

```json
{
  "song": "Heroes",
  "artist": "David Bowie",
  "genre": "rock",
  "era": "1970s",
  "tone_type": "distorted",
  "part": "riff",
  "amp_settings": { "gain": 6, "bass": 5, "mid": 6, "treble": 6, "presence": 5, "reverb": 3 },
  "original_gear": { "amp": "Hiwatt (with Hiwatt cabs) — feedback-driven sustain", "notes": "Robert Fripp played a Les Paul Custom ..." },
  "effects": ["fuzz", "reverb"],
  "pickup": "neck/bridge (sustained feedback)",
  "confidence": 0.74,
  "sources": ["https://www.guitarplayer.com/..."],
  "url": "https://guitartoneadapt.com/tone/heroes--david-bowie--riff--distorted--guitar/"
}
```

| Field | Meaning |
|---|---|
| `song`, `artist` | The track and performer |
| `genre`, `era` | Rough genre and recording decade |
| `tone_type` | `clean`, `distorted`, or `bass` |
| `amp_settings` | Starting EQ on a 0–10 scale |
| `original_gear` | The amp/guitar used on the record (best-available research) |
| `effects`, `pickup` | Signal-chain notes |
| `confidence` | 0–1 — how well-documented the entry is (estimates are labelled low) |
| `sources` | URLs the entry was researched from (interviews, rig rundowns, gear sites) |
| `url` | The full breakdown on guitartoneadapt.com |

## Notes & caveats

- Amp settings are **community-researched starting points**, not official recall sheets. Real tone depends on your specific gear; use these as a launch pad and trust your ears.
- `confidence` flags how solid each entry is. Low-confidence entries are educated estimates and say so.
- Every entry links back to a full breakdown (how the riff is played, FAQ, the rig) at [guitartoneadapt.com](https://guitartoneadapt.com).

## Using it

Great for: tone-matching tools, music ML, "what amp settings for X" lookups, data journalism about how guitar tone has evolved. (We did the latter — see [how guitar tone changed over 60 years](https://guitartoneadapt.com/guitar-tone-by-decade/).)

## License

[CC BY 4.0](LICENSE) — free to use, share and adapt, **with attribution**. Please credit *GuitarToneAdapt (https://guitartoneadapt.com)* and link back where practical.

---

Want any song's tone dialled in for **your** rig? → **[guitartoneadapt.com](https://guitartoneadapt.com)** (free, no signup)
