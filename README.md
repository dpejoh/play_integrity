# play_integrity
A Step-by-Step Guide to Pass Play Integrity

---
## For Newbies

- This guide changes often, so it might not always work perfectly for you. If you hit a problem, you might need to do a little extra searching online.
- Google removed the old SafetyNet checks. Now, to get Strong Integrity, you need a **valid keybox**

## Very Important To Know

- A **valid keybox** is very hard to find. A few people might try to sell them, but most are **scammers** or they'll sell you a leaked one that Google quickly blocks. So, to get integrity now, you usually need to use **spoofing**. You can do this with `TSupport Advance`, `PIF Inject`, or **manually**. Just know that spoofing doesn't always guarantee any type of integrity. Sometimes you might get **Basic** and other times **Strong**, even with the same setup. You'll likely need to try many times until it works.

- Some people suggest changing your **Play Store** to an older version (below v46) or using a modified one. I don't recommend this. You can't know if a modded version is safe or not. If you still want to try these methods, be very careful because there are risks. For more info, you might want to check out [Yuri's Telegram channel](https://t.me/yuriiroot).

---

## Requirements

* Rooted device
* Must have a **valid keybox**

### Required Magisk Modules

* [Zygisk Next](https://github.com/Dr-TSNG/ZygiskNext/releases)
* ~~[PIF (Play Integrity Fix)](https://github.com/chiteroman/PlayIntegrityFix/releases)~~ - **Discontinuted**
* [PIF Fork](https://github.com/osm0sis/PlayIntegrityFork)
* [PIF Manual Inject](https://github.com/KOWX712/PlayIntegrityFix/releases) For turning on **SpoofVendingSDK**
* [TrickyStore](https://github.com/5ec1cff/TrickyStore/releases)
* [Tricky Store Addon](https://github.com/KOWX712/Tricky-Addon-Update-Target-List) - Required for **KSU**, helpful for **Magisk**
* [TSupport Advance](https://t.me/CitraIntegrityTrick) - sets up a **fingerprint** and a **keybox** and some other stuff for you. However, if it doesn't work, you'll need to find a different keybox.
* [Shamiko](https://github.com/LSPosed/LSPosed.github.io/releases)

### Optional
* [BetterKnownInstalled](https://github.com/Pixel-Props/BetterKnownInstalled) - For solving **UNKNOWN_INSTALLED** issue
* [Integrity Box](https://github.com/MeowDump/Integrity-Box) – For getting a valid keybox and the **Strong Integrity**

### Apps

* [Play Integrity API Checker](https://play.google.com/store/apps/details?id=gr.nikolasspyr.integritycheck&hl=en)
* [KSUWebUI](https://github.com/5ec1cff/KsuWebUIStandalone) - For `TS Addon`

---

## Steps

### 1. Ensure Root Access

* Use **Magisk**, **KernelSU**, or another method to root your device.

### 2. Flash the Magisk Modules (In This Order)

1. `Zygisk Next`
2. `PIF Fork`
3. `Shamiko`
4. `TrickyStore`
5. `Tricky Store Addon`
6. `TSupport Advance` or `Integrity Box` (don't install them in the same time)
7. In `Tsupport Advance`, the **FP updater** script will run first. If you're new to the configuration or unsure, select "yes" for all options.

### 3. Reboot your device after flashing the modules.

## Configuring Tricky Store

### With TSupport Advance

After rebooting:

- Open **Magisk**.
- Click on **Actions**.
- Select **EBox Updater**.
- Let it set a **Keybox** for you.
- Select "yes" to all options if you're unsure about what you need to do.

### Manually

> Only required if you didn't install **TSupport Advance** or **Integrity Box**.

1. Use a file manager that supports root file operations like **ZArchiver** or **MT Manager**
2. Navigate to the path:

   ```
   /data/adb/tricky_store
   ```
3. Replace or edit the following files:

   * `target.txt`
   * `keybox.xml`

### Alternaltive method

- Update the **keybox** and the **target list** using `Tricky Store Addon` in `KSUWebUI`

> You must put a **valid keybox** or at least one that can get you **device integrity**, like the **AOSP keybox**.
> For the **target file**, you can customize it using a text editor or **KSUWebUI**.

## PIF Manual Inject

- If you can't get at least **Basic integrity**, try the `PIF Manual Inject` module, here are the steps:
1. Install the **module**
2. In `KSUWebUI`, choose `Play Integrity Fix [INJECT]`.
3. Turn on `Spoof sdk version to Play Store`
4. You can also turn on other **spoof** options, but you don't have to.

---

## Check Integrity Status

1. Open the **Play Integrity API Checker** app.
2. Tap **"Check"**.
3. Wait for the results.

You should pass:

* ✅ **Basic Integrity**
* ✅ **Device Integrity**
* ✅ **Strong Integrity** *(only with a valid keybox)*

---

> ⚠️ **Note:**
> The `keybox.xml` file can be revoked by Google at any time.
> You’ll need to:
> * Update it periodically
> * Recheck your Play Integrity status regularly
