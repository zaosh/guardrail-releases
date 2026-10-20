# Guardrail: install and set up

Guardrail blocks apps you pick, enforces daily limits, and blocks Instagram Reels / YouTube Shorts scrolling.
Changing your rules to be *less* strict needs a **lock code** held by someone you trust. It works fully offline:
the app has no internet permission, and nothing leaves your phone.

## 1. Install

1. Download `guardrail-<version>.apk` and its `.sha256` file from the Releases page.
2. Optional: check the file. On a computer: `sha256sum -c guardrail-<version>.apk.sha256`.
3. Open the APK on your phone. Android asks you to allow installs from the app you opened it with (browser or Files).
   Allow it, then tap **Install**. If Play Protect warns about an unknown app, choose **Install anyway**.

## 2. Set up (Guardrail walks you through it)

1. **Allow restricted settings.** Settings → Apps → Guardrail → ⋮ (top right) → **Allow restricted settings**.
   Android 13+ blocks Accessibility for apps installed outside the Play Store until you do this. If you don't see the option, skip it.
2. **Turn on the Accessibility service.** Settings → Accessibility → Downloaded apps → Guardrail → On.
   Guardrail reads which app and screen are open so it can tell Reels from DMs. It saves no messages or screen content.
3. **Let it run in the background.** Settings → Apps → Guardrail → Battery → **Unrestricted**
   (wording differs by phone). Otherwise the phone may stop Guardrail to save power.
4. **Usage access (optional).** Lets Guardrail count time spent while it was off.
5. **Pick apps and rules** on Home, then set up the **Lock** in Settings:
   - Guardrail shows a 16-character **lock code once**. Copy it and send it to the person you trust.
     They keep it; **delete your copy** from the chat afterwards. You can't see it again.
   - Confirm "I've sent it". The lock is now on.
   - Turn on **Device Admin** when asked, so Guardrail can't be force-stopped or uninstalled casually.

## 3. Using it

- Making rules stricter is always free. Making them looser (removing an app, raising a limit, turning the lock off,
  uninstalling) needs the lock code. Ask your partner, enter it, and you have 10 minutes to make changes.
- **Settings** shows what is working on your phone (blocking service, usage access, guarded pages). Items marked Off tell you what is missing.

## What may not work on your phone

- The **Settings guard** (stops you opening Guardrail's own Settings pages to switch it off) is built for OnePlus phones.
  Elsewhere Settings pages aren't guarded; Device Admin still blocks Force stop and plain uninstall.
- Instagram and YouTube change their screens. After an update, Guardrail may not recognise a screen. It then falls back to a
  **30-minute daily cap** on that app until a new Guardrail version supports it. That is expected, not a bug.
- Browsers: instagram.com / youtube.com in a browser are not covered yet.

## Updating

There are no automatic updates (the app can't go online). When a new version is announced, download the new APK and open it:
it installs over the old one and **keeps your rules and lock**. Never uninstall to update. Settings shows your version.

## If you're stuck

- **Lost the lock code:** contact whoever gave you Guardrail. They can reset it from a computer with USB debugging.
- **Don't uninstall.** It needs the lock code, and it removes your setup.
