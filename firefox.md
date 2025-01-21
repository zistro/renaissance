# Tips to make firefox faster

## These are the tweaks I(flemtone,r/EverythingLegal) use to reduce the memory in Firefox.

### Type about:config in the address bar and click OK to continue, then change the following settings:

* Set this to false if you have 2gb or under to stop saving pages in memory

> browser.cache.memory.enable

* A large memory cache isn't needed so 512mb is more than plenty for general browsing.

> browser.cache.memory.capacity (512000)

* Disable disk cache to save read/write to drive which can slow things down.

> browser.cache.disk.enable (false)

* Disable prefetch to stop browser making automatic connections for all links.

> network.prefetch-next (false)

* Pages loaded are stored in memory for back button usage, set to 0 to use only 32mb.

> browser.sessionhistory.max_total_viewers (0)

* Session restore save interval if browser crashes, default is every 15 seconds, change to more sensible value.

> browser.sessionstore.interval (600000)

* How many pages are saved in sessionstore above.

> browser.sessionhistory.max_entries (5)

* If you dont use Firefox Pocket then you can disable.

> extensions.pocket.enabled (false if not using pocket)

* If you dont use devtools then you can disable F12 access.

> devtools.f12_enabled (false if not using dev tools)

* Disabling accessibility features improves page load and lowers memory usage.

> accessibility.force_disabled (1 if not using accessibility options)

* Also install uBlock Origin add-on to help speed up site loading and remove adverts, if having YouTube playback issues enable Annoyance filters, make sure Ambience mode in video setting is turned off and set the following setting in about:config to true:

> media.ffmpeg.vaapi.enabled (true)


Thanks
