### Sett begrensninger på npm og uv
1. Gå til workspacet for M2. 
2. Oppdater uv i backend til å ikke tillate pakker som er nyere enn 7 dager. (Oppdater backend/pyproject.toml under "[tool.uv]")
3. Oppdater npm i frontend til å ikke tillate pakker som er nyere enn 7 dager. (Legg til en ny fil ".npmrc", og en config linje i den filen)
4. Legg til, commit og push filene til repoet.

### Herde Frontend og Backend images pakkeinstallasjon
1. Åpne et codespace på branch "fix/use-hardened-images", ved å gå til https://github.com/msilabben/<ditt M2 repo>/tree/fix/use-hardened-images > "Code" > "create workspace on fix/use-hardened-images"
2. Åpne en PR fra "fix/use-hardened-images" til main og verifiser at denne blir grønn
