# VieNeu Voice Profile

This directory contains a zero-shot VieNeu voice profile.

## Files

- `reference.wav` - cleaned reference audio
- `reference.txt` - exact transcript of reference audio
- `voice_codes.npy` - encoded VieNeu voice codes
- `profile.json` - profile metadata

Test samples (`test_*.wav`) are generated in the repository
root on each run and are not tracked long-term here.

## Model

VieNeu TTS 2.7.0

## Usage

Load `voice_codes.npy` and use it with:

```python
audio = tts.infer(
    text="Nội dung cần đọc",
    ref_codes=ref_codes,
    ref_text=reference_text,
)
```
