<h1>
<sub>
<img src="https://raw.githubusercontent.com/conceptualspace/yet-another-speed-dial/master/src/icons/icon32.png" height="32" width="32">
</sub>
Yet Another Speed Dial
</h1>

<h1>
<a href='https://addons.mozilla.org/en-US/firefox/addon/yet-another-speed-dial/'><img alt='Get it for Firefox' src='https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/badges/ff-badge.png'/></a> <a href='https://chrome.google.com/webstore/detail/yet-another-speed-dial/imohnlganmafcmidafklgkgfgaagiohn'><img alt='Get it for Chrome' src='https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/badges/chrome-badge.png'/></a> <a href='https://microsoftedge.microsoft.com/addons/detail/kachajgmekhiajhbbfpfhbmonmpnpiee'><img src='https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/badges/microsoft-badge.png' alt='English badge' style='width: 166px; height: 60px;'/></a>
</h1>

A modern, cross-browser speed dial that respects your privacy, inspired by Opera

- Automatically generates thumbnails and screenshots, or add your own.
- Uses the native bookmarks library so speed dials can be synced by the browser.
- Sortable with drag and drop
- Supports folders
- Simple and fast UI
- No ads, trackers, or BS :)

![alt tag](https://github.com/conceptualspace/yet-another-speed-dial/raw/master/assets/screenshot.png)

## FAQ:

#### Can I use different images for the speed dials?
Yes! Just right-click the speed dial and select Edit.

#### One of my site thumbnails disappeared?
YASD loads thumbnails using the Open Graph standard. This keeps those thumbnails up to date automatically, but if a website removes the image it may no longer load in YASD. To fetch new images, simply right-click the dial and select "Refresh thumbnails".

#### Why does YASD require the "access your data for all websites" permission?
This is required for YASD to capture an image of the website for the thumbnail. **YASD accesses absolutely no other data for any reason whatsoever**. These two features (visual thumbnails and user privacy) were the primary motivation for creating YASD. Note, YASD still works if you deny this permission, just without capturing thumbnails. You can find the YASD privacy policy here: https://conceptualspace.net/privacy.md

#### Why is YASD showing CPU usage in the Chrome task manager?
While the actual CPU usage is very low (confirm using your OS task manager), some cycles are used to elimate jankiness. YASD uses a high performance rendering engine (GSAP) to keep user ineractions and animations smooth. The usage is 0 when YASD is not in focus.

#### Can I open speed dial links in Firefox Containers?
Yes, just use <kbd>Shift</kbd> + <kbd>Right-click</kbd> on the speed dial to access the default context menu.

#### Why isn't the address bar focused (active) by default on the new tab / home page?
This is a bug in Firefox: https://bugzilla.mozilla.org/show_bug.cgi?id=1411209

## Building

chrome: remove `chrome_settings_overrides` and `browser_specific_settings` manifest keys
