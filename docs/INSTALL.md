# Install Guide

Full walkthrough for jailbreaking your Xbox 360 with `GhostGirlRepack`.

> ⚠️ **Read this entire guide before starting.** Skipping steps will
> cause the exploit to fail — especially the console settings, the
> USB port choice, and the timing before power-on.

---

## Before You Begin

### Check Your Console

Your console must support one of these exploits:

- **ABadUpdate**
- **ABadAvatar**

If it doesn't, this guide won't work for you yet. See the
[Compatibility table](../README.md#-compatibility).

### What You Need

| Item | Notes |
|---|---|
| Xbox 360 console | Jailbreakable |
| USB stick | FAT32, under 32GB |
| PC | To prepare the USB stick |
| `GhostGirlRepack V 1.3.9.zip` | From Releases |

### Warnings

- **Back up your saves** before starting
- **Read the DISCLAIMER** — modding voids warranties
- **Do not unplug the console** during the process
- **Permanent softmod is NOT recommended** right now

---

## Step 1 — Prepare the USB Stick

1. Insert a USB stick into your PC.
2. Back up anything important on it.
3. Format it to **FAT32**:

   **Windows:**
   - File Explorer → Right-click USB → Format
   - File system: **FAT32**
   - Click Start

   **Linux:**
   ```
   sudo mkfs.vfat -F 32 /dev/sdX
   ```
   Replace `sdX` with your USB device (check with `lsblk`).

   **macOS:**
   - Disk Utility → Select USB → Erase
   - Format: **MS-DOS (FAT)**
   - Click Erase

4. Confirm the format completed successfully.

---

## Step 2 — Extract GhostGirlRepack

1. Download `GhostGirlRepack V 1.3.9.zip` from Releases.
2. Extract it on your PC.
3. Inside, find the folder named **`GhostGirlRepack`**.
4. Open that folder.

### What's Inside

You should see:

```
GhostGirlRepack/
├── Apps/
├── BadUpdatePayload/
├── Content/
├── Dash/
├── HvP2.xex
├── JRPC2.ini
├── JRPC2.xex
├── launch.ini
├── name.txt
├── README - Credz and sources.txt
├── README - GhostGirlRepack.txt
├── README - XeUnshackle.txt
├── RPC.xex
├── xbdm.ini
└── Xbdm.xex
```

If it doesn't match, re-extract the zip.

---

## Step 3 — Copy Files to USB

1. **Open the `GhostGirlRepack` folder.**
2. **Select ALL items inside** — both folders and files.
3. **Copy them.**
4. **Paste them directly onto the root of the USB stick.**

   ⚠️ Do **not** copy the `GhostGirlRepack` folder itself. Only
   the contents inside it.

### ✅ Correct USB Layout

```
USB:\
├── Apps/
├── BadUpdatePayload/
├── Content/
├── Dash/
├── HvP2.xex
├── JRPC2.ini
├── JRPC2.xex
├── launch.ini
├── name.txt
├── README - Credz and sources.txt
├── README - GhostGirlRepack.txt
├── README - XeUnshackle.txt
├── RPC.xex
├── xbdm.ini
└── Xbdm.xex
```

### ❌ Wrong USB Layout

```
USB:\
└── GhostGirlRepack\              ← WRONG
     ├── Apps/
     ├── HvP2.xex
     └── ...
```

If you see a `GhostGirlRepack` folder on your USB stick, delete it
and redo Step 3 by selecting the **files inside** instead.

5. Do **not** rename any files after copying them.
6. Safely eject the USB stick.

---

## Step 4 — Prepare Console Settings ⚠️ IMPORTANT

**Before plugging the USB stick into the console**, change these
settings. If you skip this, the jailbreak will not work.

### 4.1 — Turn Off Wi-Fi

1. Power on the console **without** the USB stick inserted.
2. Go to **Settings → System → Network Settings**.
3. Disconnect from any wireless network.
4. Turn Wi-Fi off completely.

### 4.2 — Turn Off Auto Sign-In

1. Go to **Settings → System → Console Settings → Startup and Shutdown**.
2. Set **Auto Sign-In** to **Off**.

### 4.3 — Power Off the Console

1. Shut down completely.
2. Wait **30 seconds**.
3. Make sure no lights are on and no fan is running.

---

## Step 5 — Plug In USB & Boot

⚠️ **Follow these steps in exact order. Timing matters.**

1. With the console fully off, plug the USB stick into the USB
   port **closest to the power button**.
2. **Wait 5 seconds.** Do not press anything.
3. Press the **power button** to turn on the console.
4. **Wait.** The jailbreak runs automatically.
5. A profile named **`abadavatar`** appears on the sign-in screen.
6. Click the **`abadavatar`** profile to sign in.
7. ✅ Console is now jailbroken.

> 💡 **If the `abadavatar` profile doesn't appear**, something went
> wrong. See [TROUBLESHOOTING.md](TROUBLESHOOTING.md).

---

## Step 6 — Verify

After the jailbreak completes, check:

- [ ] Console booted with `abadavatar` profile visible
- [ ] You can sign in to that profile
- [ ] Homebrew apps run

If any step fails, see [TROUBLESHOOTING.md](TROUBLESHOOTING.md).

---

## Step 7 — Keeping It Jailbroken

The jailbreak is **temporary** — it only lasts as long as the
console stays powered on.

When you power off, you must repeat **Steps 4 and 5** to
re-jailbreak.

> **Note:** Permanent softmod is possible with GhostGirlRepack
> but **NOT recommended** at the moment. See the warning at the
> top of the main README.

---

## Still Stuck?

- See [TROUBLESHOOTING.md](TROUBLESHOOTING.md)
- Ask in Discord `#help`
- Open an issue with the `question` label

Include:
- Console model and revision
- What step failed
- What you expected vs. what happened
