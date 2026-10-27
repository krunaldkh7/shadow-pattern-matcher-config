# Shadow Pattern Matcher — remote ad config

The app downloads `ads.json` from this repo every time it starts.
Edit it here and commit; users get the change the next time they open the app
(GitHub's raw CDN can take a few minutes to refresh).

- `show_ads`: `true` shows ads, `false` turns every ad off.
- `banner_ad_unit_id`, `interstitial_ad_unit_id`: Android AdMob unit IDs.
- `ios`: the same keys for the iOS unit IDs.
- `interstitial_every_n_levels`: full-screen ad after every N solved levels (`0` = never).

The current IDs are Google's public **test** IDs.
