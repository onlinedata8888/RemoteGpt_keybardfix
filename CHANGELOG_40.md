# Remote2 40
- Keyboard: phone box ab TV ke search/text field ko mirror karta hai (TV me pehle se likha text, jaise 'a', phone me dikhta hai) aur har edit pura value bhejta hai -> delete / clear ab kaam karta hai. TV khud text field khole to keyboard apne aap khulta hai.
- Empty-text bug fix (IME cursor -1 encode ho raha tha).
- Play Store button: Google TV ke liye sahi launch intent (TvMainActivity). Agar TV ne kuch nahi kiya to 8 sec ke andar dobara tap = agla tareeka.
- App/Play Store launch: har baar toast dikhta hai ki kaun sa tareeka (1st, 2nd, 3rd...) chal raha hai.

## Gamepad compatibility fix — 2026-10-03
- Corrected HID gamepad button usages to the standard Android/Xbox-style order: A/B/X/Y, L1/R1/L2/R2, Select/Start/Home/L3/R3.
- Corrected HID hat-switch encoding to 0..7 for directions with 8 as the null/released state.
- Normalized outgoing HID report bytes and invalid hat values before transmission.
- Kept the existing gamepad UI, remote, keyboard and mouse behavior unchanged.
