# Keep_Target_SoC.json

Flow umožňuje pomocí změny AC Grid Point udržovat nastavené SoC. Důvodem vzniku toho skriptu bylo velké množství slunečních dní za sebou,
kdy baterie se během několika hodin nabila a pak se "trápila" po zbytek dne na 100%, což má určitě negativní vliv na její životnost.

Flow umožňuje ovládání jak přes Dasboard Node-RED ve VRM, tak i přes MQTT brokera v Cerbo.

Pro MQQT nezapomeňte pozměnit v uzlech čtení stavů a zápisu stavů instalační ID, aby odpovídalo Vaší instalaci.

Pro Home Assistant přikládám ukázkovou konfiguraci, musíte si opět upravit Topicy dle své instalace.

Problémem regulace je poměrně dlouhá zpětná vazba, takže regulace není ideální, při častých změnách odběru/výroby relativně dlouho kmitá,
ale u baterky 28,4 kWh je přesto schopno držet po zbytek dne na procento přesně. 
