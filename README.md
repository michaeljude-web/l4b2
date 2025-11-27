# Pause Windows Update via Registry Editor

This guide shows how to pause Windows Updates by modifying the registry.

## Steps

1. Press `Win + R` to open Run dialog.
2. Type `regedit` and press Enter to open Registry Editor.
3. Navigate to `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\WindowsUpdate\UX\Settings`
4. Right-click **Settings** → New → DWORD (32-bit) Value → Name: `FlightSettingsMaxPauseDays`
5. Double-click the new value → Decimal → enter `50000` → OK
6. Open **Settings → Windows Update** and select a Pause Updates date

> [!NOTE]
> The pause value (`50000`) allows pausing updates for a very long time
