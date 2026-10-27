# Shadow Pattern Matcher — remote ad config

The app downloads `ads.json` from this repo every time it starts.
Edit it here and commit; users get the change the next time they open the app
(GitHub's raw CDN can take a few minutes to refresh).

| Key | What it does |
|---|---|
| `show_ads` | `true` shows ads, `false` turns every ad off. |
| `banner_ad_unit_id` | Banner at the bottom of menu screens. |
| `interstitial_ad_unit_id` | Full-screen ad between levels. |
| `rewarded_ad_unit_id` | "Watch an ad" hint that keeps your bulb. |
| `app_open_ad_unit_id` | Full-screen ad when the player returns to the app. |
| `native_ad_unit_id` | Ad card between the gallery cards. |
| `interstitial_every_n_levels` | Interstitial after every N solved levels (`0` = never). |
| `interstitial_start_after_level` | No interstitials until this many levels are solved. |
| `interstitial_min_interval_seconds` | Minimum time between two interstitials. |
| `app_open_cooldown_minutes` | Minimum time between two app-open ads. |
| `free_hints_per_level` | Hints per level that only cost a bulb; after that a hint asks for an ad. |
| `ios` | The same unit-ID keys for iOS (top-level IDs are Android). |

To turn off one format, delete its unit ID. The current IDs are Google's public **test** IDs.
