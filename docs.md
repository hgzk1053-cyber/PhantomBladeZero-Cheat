# Troubleshooting

## Antivirus flags INSTALL.exe

False positive. Patchers modify game files in `steamapps/common`, which triggers AV heuristics. Add the game folder to exclusions:

1. Windows Security → Virus & threat protection → Manage settings → Exclusions → Add folder
2. Point to your Phantom Blade Zero folder

If AV deletes the file during extraction, temporarily disable real-time protection, extract, re-enable.

## Game won't launch after patch

Run `INSTALL.exe` → **Restore Backup**. This reverts `Engine.ini` and the shader cache to pre-patch state.

If the game still won't launch, verify game files on Steam/Epic (this overwrites patched files).

## Shader compile still slow on first launch

Delete the cache and relaunch:

```cmd
del /q "%LOCALAPPDATA%\PhantomBladeZero\shadercache\*"
