# Shadow Pattern Matcher — remote ad config

The app downloads `ads.json` from this repo every time it starts.
Edit it here and commit; users get the change the next time they open the app
(GitHub's raw CDN can take a few minutes to refresh).

| Key | What it does |
|---|---|
| `show_ads` | `true` shows ads, `false` turns every ad off. |
| `banner_ad_unit_id` | Banner at the bottom of menu screens. |
| `interstitial_ad_unit_id` | Full-screen ad between levels. |
| `rewarded_ad_unit_id` | Extra hints: once a level's 3 bulbs (top) or 3 free hints (bottom) are used, a tap offers a rewarded video. |
| `app_open_ad_unit_id` | Full-screen ad when the player returns to the app. |
| `native_ad_unit_id` | Ad card between the gallery cards. |
| `interstitial_every_n_clicks` | Interstitial after every N taps on menu screens. Taps on the game screen never count, and the ad never opens on top of a level (`0` = never). |
| `interstitial_every_n_levels` | Interstitial after every N solved levels (`0` = never). |
| `interstitial_start_after_level` | Level-based interstitials wait until this many levels are solved. |
| `interstitial_min_interval_seconds` | Minimum time between two interstitials. |
| `app_open_cooldown_minutes` | Minimum time between two app-open ads. |
| `ios` | The same unit-ID keys for iOS (top-level IDs are Android). |

To turn off one format, delete its unit ID. The current IDs are Google's public **test** IDs.
