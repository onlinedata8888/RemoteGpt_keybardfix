# Keyboard protocol fix

- Corrected Android TV Remote v2 `RemoteEditInfo.insert` from `1` to `0`.
- Keeps IME counter/field counter learned from TV `remote_ime_batch_edit` responses.
- Preserves full-field text sync and DEL fallback.
- Does not change remote/gamepad UI mappings.

The Android TV Remote v2 batch-edit schema uses `RemoteEditInfo.insert` with the text-field object; reference implementations/examples send `insert = 0` for text injection.
