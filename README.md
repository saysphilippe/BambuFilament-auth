# BambuFilament-auth

Brukerlisten for [BambuFilament](https://saysphilippe.github.io/BambuFilament/): navn, farger, rolle og
innloggingsnøkler i `users.json`.

Repoet er offentlig fordi nettsiden må kunne lese brukerlisten før noen er logget inn. Innloggingsnøklene
er GitHub-tokenen kryptert per bruker (AES-256-GCM, nøkkel fra passordet med PBKDF2-SHA256, 600 000
runder). Selve dataene (spoler, AMS, bibliotek, venteliste) ligger i et privat repo og kan bare leses
med tokenen etter innlogging.
