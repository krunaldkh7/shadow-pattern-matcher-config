# Shadow Pattern Matcher — remote ad config

The app downloads `ads.json` from this repo every time it starts.
Edit it here and commit; users get the change the next time they open the app
(GitHub's raw CDN can take a few minutes to refresh).

| Key | What it does |
|---|---|
| `show_ads` | `true` shows ads, `false` turns every ad off. |
| `banner_ad_unit_id` | Banner at the bottom of menu screens. |
| `interstitial_ad_unit_id` | Full-screen ad: after random menu taps, and as the price of a hint once a level's free hints are used up. |
| `rewarded_ad_unit_id` | Reward video behind the in-game **Skip** button: watch it to skip a level. |
| `rewarded_interstitial_ad_unit_id` | Offered on the solved card when bulbs were spent: a 5-second intro (with "No thanks"), then an ad that restores all 3 bulbs. |
| `app_open_ad_unit_id` | Full-screen ad when the player returns to the app. |
| `native_ad_unit_id` | Ad card between the gallery cards. |
| `interstitial_taps_min` / `interstitial_taps_max` | Interstitial after a random number of taps (between min and max) anywhere outside the game screen. A short "Loading ad…" screen shows first. Taps on the game screen never count (`0` for both = never). |
| `interstitial_every_n_levels` | Interstitial after every N solved levels (`0` = never). |
| `interstitial_start_after_level` | Level-based interstitials wait until this many levels are solved. |
| `interstitial_min_interval_seconds` | Minimum time between two interstitials. |
| `app_open_cooldown_minutes` | Minimum time between two app-open ads. |
| `ios` | The same unit-ID keys for iOS (top-level IDs are Android). |

To turn off one format, delete its unit ID. The current IDs are Google's public **test** IDs.
