# Simplefox
A simple list of [about:config](https://support.mozilla.org/en-US/kb/about-config-editor-firefox) tweaks to enhance [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/).

Improves privacy and quality of life while maintaining a heavy emphasis on usability, ie.:

- disables telemetry, AI and speculative loading
- enables Strict Tracking Protection and DNS over HTTPS (with additional ad, tracker and malware blocking)
- opts out of experiments and crash reports

## Instructions
0) Create a backup profile. Not needed, but recommended.
1) Download the `user.js` or `casual.js` file. (Rename `casual.js` to `user.js` after downloading!)
2) In Firefox, type `about:profiles` in the URL bar and press **Enter**.
3) For the profile you want to use, click **Open Folder** in the **Root Directory** section.
4) Move the `user.js` file into the folder.
5) Restart Firefox.
6) Optionally install the [uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/) ad and content blocker.

## Which one is for me, `user.js` or `casual.js`?
While very similar, `casual.js` has some minor changes compared to `user.js` to ensure reliability.

1) Enables "Fix major site issues" under Enhanced Tracking Protection.
2) Removes alternative geo service.
3) Switches from "Max Protection" to "Increased Protection" under DNS over HTTPS.
4) Enables crash reporting.

`user.js` is very stable (personally never had any problems), but `casual.js` further ensures it.

Whichever you choose, you can always tweak it to your liking. [Betterfox](https://github.com/yokoffing/Betterfox) has great lists of common changes: [Common Overrides](https://github.com/yokoffing/Betterfox/wiki/Common-Overrides) and [Optional Hardening](https://github.com/yokoffing/Betterfox/wiki/Optional-Hardening).

## Heavily opinionated settings

1) `user.js`: Geo service provider - [BeaconDB](https://beacondb.net/)
2) **Both**: DNS over HTTPS provider - [Mullvad](https://mullvad.net/en) (anti ad, tracker and malware [preset](https://mullvad.net/en/help/dns-over-https-and-dns-over-tls))
3) `casual.js`: Crash reporting enabled.

Should you prefer some other service providers, the respective settings have been located at the top of both `user.js` and `casual.js` files.

Crash reporting is enabled in `casual.js` to stay consistent with the philosophy of a more stable user experience.

## What is a `user.js`?
`user.js` is a configuration file you can use to change Firefox' [about:config](https://support.mozilla.org/en-US/kb/about-config-editor-firefox) settings in bulk.

Simplefox' `user.js` is a curated list of simple changes to improve the already great Firefox experience.

## How is this different from Betterfox or Arkenfox?
[Betterfox](https://github.com/yokoffing/Betterfox) and its parent project [Arkenfox](https://github.com/arkenfox/user.js) both use a `user.js` to improve the Firefox experience.

Simplefox is a shrunk fork of Betterfox to keep things simpler, mainly for my personal use.

## Will this hide me on the internet?
No. If you want or need anonymity, use the [Tor Browser](https://www.torproject.org/).