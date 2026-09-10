# System-Setup "Legacy Systeme verbessern mit Agentic Coding" Workshoptage Rapperswil 2026

## sbx

in a dir on your machine do:
```
PROJ_DIR=$(pwd)
git clone https://github.com/innoq-legacy-modernization2609/roller-for-workshop.git roller
cd roller
sbx settings set kit.allowedSources '["docker.io/","github.com/docker/","github.com/innoq-legacy-modernization2609/"]'

sbx run \
  --kit "git+https://github.com/docker/sbx-kits-contrib.git#dir=pi" \
  --kit "git+https://github.com/innoq-legacy-modernization2609/sbx-kits.git#dir=heribert-ai-gateway" \
  pi
```

## Cloud environment
see https://crucible.ch.innoq.io/t/17466581b087289a/

Im Web den VS Code öffnen. Das rechte Panel (Chat) schliessen. Das Terminal von unten hereinziehen.
git clone https://github.com/innoq-legacy-modernization2609/roller-for-workshop.git roller
cd roller
pi


## Letzter Schritt in PI
/login litellm -> API Key eingeben
/model -> eu.glm-5.3 auswählen
/thinking -> medium
