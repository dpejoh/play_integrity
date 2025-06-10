# play_integrity
A Step-by-Step Guide to Pass Play Integrity

## 🧰 Requirements

### Rooted Device

* Must be rooted using **Magisk**

### Required Magisk Modules

* [Zygisk Next](https://github.com/Dr-TSNG/ZygiskNext/releases)
* ~~[PIF (Play Integrity Fix)](https://github.com/chiteroman/PlayIntegrityFix/releases)~~ **Discontinuted**
* [PIF Fork](https://github.com/osm0sis/PlayIntegrityFork)
* [TrickyStore](https://github.com/5ec1cff/TrickyStore/releases)
* [Tricky Store Addon](https://github.com/KOWX712/Tricky-Addon-Update-Target-List) Required for **KSU**, helpful for **Magisk**
* [Shamiko (optional but helpful)](https://github.com/LSPosed/LSPosed.github.io/releases)

### Keybox Providers (Choose One)

* [TSupport Advance (recommended)](https://t.me/CitraIntegrityTrick)
* [Integrity Box](https://github.com/MeowDump/Integrity-Box) – supports **Strong Integrity**

### Apps

* [Play Integrity API Checker](https://play.google.com/store/apps/details?id=gr.nikolasspyr.integritycheck&hl=en)
* [KSUWebUI](https://github.com/5ec1cff/KsuWebUIStandalone) For **TS Addon**
---

## 🛠️ Steps

### 1. Ensure Root Access

* Use **Magisk**, **KernelSU**, or another method to root your device.

### 2. Flash the Magisk Modules (In This Order)

1. `Zygisk Next`
2. `PIF` or `PIF Fork`
3. `Shamiko` *(optional but recommended)*
4. `TrickyStore`
5. `TSupport Advance` or `Integrity Box`

### 3. Reboot your device after flashing the modules.
---

## Configuring Tricky Store

### With TSupport Advance

After rebooting:

- Open **Magisk**.
- Click on **Actions**.
- Select **EBox Updater**.
- Let it set a **Keybox** for you.
- Set `spoofvendingsdk` to `true`.

> ⚠️ Note: This step may not work in the future, but for now, it works to get integrity.

### Manually

> Only required if you didn't install **TSupport Advance** or **Integrity Box**.

1. Open **ZArchiver**.
2. Go to `Settings > ROOT` and enable:

   * File operations
   * Fix SELinux content
3. Grant **root access** to ZArchiver.
4. Navigate to the path:

   ```
   /data/adb/tricky_store
   ```
5. Replace or edit the following files:

   * `target.txt`
   * `keybox.xml`

> You must put a **valid keybox** or at least one that can get you **device integrity**, like the **AOSP keybox**.
> For the **target file**, you can customize it using a text editor or **KSUWebUI**.
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

* Update it periodically
* Recheck your Play Integrity status regularly
