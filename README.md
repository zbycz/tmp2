# Cvičební timer

Intervalový timer na cvičení – jedna statická stránka, nasazená na GitHub Pages.

- **Zvuk na iOS**: pípání jede přes Web Audio, s `navigator.audioSession = 'playback'`, tichou smyčkou v `<audio>` a fallbackem na `<audio>` elementy, aby ho iOS neztlumil. Boční přepínač musí být na zvonění.
- **Displej nezhasne**: dokud timer běží, drží se Screen Wake Lock (iOS 16.4+, Android Chrome, desktop).
- **Na plochu**: manifest + service worker, takže jde přidat na plochu a běží fullscreen i offline.
