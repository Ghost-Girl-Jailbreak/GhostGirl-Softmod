# Troubleshooting

Common problems and how to fix them.

If your issue isn't listed here, see **Still Stuck?** at the bottom.

---

## USB & File Issues

### Console does not detect the USB stick

**Check:**

- Is the stick formatted to **FAT32**? (exFAT and NTFS won't work)
- Try a different USB port
- Try a different USB stick
- Is it larger than **32GB**? Some consoles struggle with large drives
- Is it fully inserted? Push it until it clicks

**Fix:**

1. Format the USB stick again to FAT32
2. Re-copy the files from `GhostGirlRepack`
3. Safely eject and reinsert

---

### Files are inside a `GhostGirlRepack` folder on the USB

**This is the most common mistake.**

**Fix:**

1. Open the `GhostGirlRepack` folder on the USB stick
2. Select **all items inside**
3. Cut them
4. Paste them at the **root** of the USB stick
5. Delete the now-empty `GhostGirlRepack` folder

See [FILE_LAYOUT.md](FILE_LAYOUT.md) for the correct layout.

---

### Files were renamed

Windows or macOS may add `(1)` to duplicate filenames.

**Fix:**

1. Delete everything from the USB stick
2. Re-copy from the original `GhostGirlRepack` folder
3. Do not rename anything

---

## Jailbreak Issues

### `abadavatar` profile does not appear

**Check:**

- Wi-Fi was **off** before booting? (Step 4.1)
- Auto Sign-In was **off**? (Step 4.2)
- Waited **30 seconds** after powering off?
- Waited **5 seconds** after inserting USB before powering on?
- USB stick in the port **closest to the power button**?
- Files at the **root** of the USB stick (not in a `GhostGirlRepack` folder)?
- Files not renamed?

**Fix:**

1. Power off completely
2. Wait 30 seconds
3. Confirm Wi-Fi is off and Auto Sign-In is off
4. Remove the USB stick, reinsert it into the port closest to the power button
5. Wait 5 seconds
6. Power on
7. Wait for `abadavatar` to appear

---

### Console boots normally but nothing happens

**Cause:** USB not detected, or timing was off.

**Fix:**

1. Power off, wait 30 seconds
2. Try a different USB port
3. Try a different USB stick (FAT32, under 32GB)
4. Re-copy files from `GhostGirlRepack` — contents only, not the folder

---

### `abadavatar` profile appears but sign-in fails

**Fix:**

1. Power off, wait 30 seconds
2. Power back on and try again
3. If it keeps failing, re-extract `GhostGirlRepack.zip` and re-copy

---

### Console signs into my normal profile instead of `abadavatar`

**Cause:** Auto Sign-In is still on.

**Fix:**

1. Go to Settings → System → Console Settings → Startup and Shutdown
2. Set Auto Sign-In to **Off**
3. Power off, wait 30 seconds
4. Follow Step 5 again

---

### Jailbreak works but Wi-Fi won't connect afterward

**Cause:** Some exploits conflict with network services if Wi-Fi is enabled during boot.

**Fix:**

1. Reboot without the USB stick
2. Re-enable Wi-Fi manually
3. You may need to re-jailbreak if you want online features

---

### Console freezes during jailbreak

**Fix:**

1. Hold the power button for 10 seconds to force power off
2. Unplug the USB stick
3. Wait 30 seconds
4. Reinsert and try again
5. If it keeps freezing, try a different USB stick

---

## Still Stuck?

- 💬 [Join the Discord](https://discord.gg/2YFyMqP6Te) — ask in `#help`
- 🐛 [Open an issue](../../issues/new) with the `question` label

Include:
- Console model and revision
- What step failed
- What you expected vs. what happened
