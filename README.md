# Go Route Sürücü (yousurucu)

Go Route Taksi sürücüləri üçün PWA/Play tətbiqi. Müştəri tətbiqi: `youtaxi`. Eyni Firebase layihəsi (`bkaugo`) və eyni kolleksiyalar:

- `taxiDriverProfiles/{uid}` — şəxsi sürücü profili (`approved` admin tərəfindən true edilir)
- `taxiDrivers/{uid}` — canlı vəziyyət (müştəri xəritəsi üçün): `online, busy, cls, lat, lng, heading, updatedAtMs`
- `taxiRides/{id}` — sifarişlər: `searching → accepted → arrived → ongoing → completed` (və ya `cancelled`)

Fayllar: `index.html` (bütün tətbiq), `manifest.json`, `sw.js`, `offline.html`, `privacy-policy.html`, `delete-account.html`,
`firestore.taxi.rules`, ikonlar, `store/` ← Play qrafikləri. Quraşdırma və Play addımları: **PLAY_STORE.md**.

Məhdudiyyət (v1): GPS yalnız tətbiq açıq və ekran oyaq olduqda göndərilir (arxa fonda izləmə Google Play-in əlavə təsdiqini tələb edir).
