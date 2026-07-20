# 真人審核音檔

建議由泰語母語者在安靜環境錄製，每題一個 MP3 或 WAV，保留自然音高，不做變調。

1. 把音檔放在此資料夾，例如 `vc_bp_001.mp3`。
2. 在 `data/audio-manifest.json` 加入題號與路徑：

```json
{
  "vc_bp_001": "assets/audio/vc_bp_001.mp3",
  "tone_lf_001": "assets/audio/tone_lf_001.mp3"
}
```

系統會優先播放這裡設定的音檔；讀取失敗時自動回退到裝置的泰語 TTS。
