# play_integrity
A Step-by-Step Guide to Pass Play Integrity

---
## 🧰 Requirements

### Rooted Device

* Must be rooted using **Magisk**

### Required Magisk Modules

* [✅ Zygisk Next](https://github.com/Dr-TSNG/ZygiskNext/releases)
* [✅ PIF (Play Integrity Fix)](https://github.com/chiteroman/PlayIntegrityFix/releases)
* [✅ TrickyStore](https://github.com/5ec1cff/TrickyStore/releases)
* [✅ Shamiko (optional but helpful)](https://github.com/LSPosed/LSPosed.github.io/releases)

### Keybox Providers (Choose One)

* 🔹 [TSupport Advance (recommended)](https://t.me/CitraIntegrityTrick)
* 🔹 [Integrity Box](https://github.com/MeowDump/Integrity-Box) – supports **Strong Integrity**

### Testing App

* 📲 [Play Integrity API Checker](https://play.google.com/store/apps/details?id=gr.nikolasspyr.integritycheck&hl=en)

---

## 🛠️ Steps

### 1. Ensure Root Access

* Use **Magisk**, **KernelSU**, or another method to root your device.

### 2. Flash the Magisk Modules (In This Order)

1. `Play Integrity Fix (PIF)`
2. `Shamiko` *(optional but recommended)*
3. `TrickyStore`
4. `TSupport Advance` or `Integrity Box`

> **Reboot your device after flashing the modules.**
> Let all modules initialize properly after rebooting.

---

## ⚙️ Configuring Tricky Store

> Only required if you didn't install **TSupport Advance** or **Integrity Box**.

1. Open **ZArchiver**.
2. Go to `Settings > ROOT` and enable:

   * ✅ File operations
   * ✅ Fix SELinux content
3. Grant **root access** to ZArchiver.
4. Navigate to the path:

   ```
   /data/adb/tricky_store
   ```
5. Replace or edit the following files:

   * `target.txt`
   * `keybox.xml`

---

## ✅ Check Integrity Status

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

* Update it periodically
* Recheck your Play Integrity status regularly

---

Let me know if you want this as a downloadable file or converted to PDF/HTML!
