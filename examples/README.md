# Examples

Sanitised versions of real automations from the house. They are **reference
material, not a drop-in package**:

- Entity IDs are generic placeholders (`lock.front_door`, `cover.all_shutters`, …).
- Anything account-specific (chat IDs, provider IDs, add-on slugs) is a `!secret`.
- Prompts are translated from the Hebrew originals. Spoken (TTS) strings stay in
  Hebrew because that is what the house actually says.
- Modern syntax (`triggers:` / `actions:` / `action:`), Home Assistant 2024.10+.

| File | What it shows |
|---|---|
| [`door-camera-ai.yaml`](door-camera-ai.yaml) | 4-frame stream analysis, JSON schema, lock-context veto, 4-way router, fallback, quiet-hours TTS |
| [`notify-household-script.yaml`](notify-household-script.yaml) | The single notification script everything goes through |
| [`home-front-alert.yaml`](home-front-alert.yaml) | Missile-alert choreography with `mode: restart` and a spoken countdown |
| [`presence-fan.yaml`](presence-fan.yaml) | PIR + mmWave fan with three independent off-paths |
| [`battery-forecast.yaml`](battery-forecast.yaml) | Days-left prediction from a 30-day drain trend |
| [`leaving-home-summary.yaml`](leaving-home-summary.yaml) | "You left home" inventory with one-tap Telegram fixes |
| [`zigbee-self-heal.yaml`](zigbee-self-heal.yaml) | Restart → verify → escalate |
| [`sun-shutter-advisor.yaml`](sun-shutter-advisor.yaml) | Ask-don't-act comfort automation |
