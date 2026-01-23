# PV017 poznámky


- [ ] Prezentace 1
    - [ ] nejsem si jistý jak správně zadefinovat riziko a uplatnění hrozby
- [ ] Prezentace 2
- [ ] Prezentace 3
- [ ] Prezentace 4
- [ ] Prezentace 5
- [ ] Prezentace 6
- [ ] Prezentace 7
- [ ] Prezentace 8
- [ ] Prezentace 9
- [ ] Prezentace 10
- [ ] Prezentace 11
- [ ] Prezentace 12

---


## Prezentace 1

### **Aktivum** (Asset) - předmět, myšlenka, informace, atd. mající pro organizaci hodnotu

- **Hmotná** - sáhnu si na něj (budovy, peníze, lidé, hardware, ...)
- **Nehmotná** - "virtuální" (software, data, patenty, autorská práva, ...)

### **Zranitelnost** (Vulnerability) - slabina využitelná ke způsobení škod/ztrát

- **CVE database** (**C**ommon **V**ulnerabilities and **E**xposures) - soupis známých zranitelností, provozováno MITRE

### **Hrozba** (Threat) - Potenciální možnost využití zranitelného místa k útoku útočníkem

- **Typy hrozeb**:
    - **Odhalení** (Disclosure) citlivých důvěrných dat, postupů, ... (např. analýza komunikačního provozu)
    - **Podvod**, klamání (Deception)
        - Falšování identity, **maškaráda** (Masquerade) - útočník vystupuje jako legitimní uživatel
        - Rozšiřování malware (Planting) - trojský kůň, vir, ...
    - **Narušení**, ničení (Disruption)
        - Neautorizovaná modifikace a využití zdrojů, man in the middle útoky, impact
    - **Vnitřní hrozby** (insider threat) - útočník je součástí zranitelné organizace
    - **Vnější hrozby** - útočník útočí odkudkoliv ze světa
- **STRIDE Framework** pro modelování hrozeb a přiklady:
    - **Spoofing**: poslání emailu pod jinou identitou, odposlechnutí WiFI jména a hesla, vykonání finanční transakce pod jinou identitou, falešná webová stránka zjišťující jména a hesla, ...
    - **Tampering**: přístup do DB skrze rozhraní pro správu (default admin credentials), změna svých zdravotních údajů v medicínské aplikaci VZP, změna stavu onboardingu
    - **Repudiation**: nelze zjistit, kdo poslal příkaz k mazání záloh
    - **Information Disclosure**: získání admin přístupu, únik dat z chybně zpřístupněného cloudového prostoru
    - **Denial of Services**:  rušení rádiových frekvencí vybrané IoT sítě
    - **Elevation of Privilege**: neoprávněné čtení dat z paměti, kde mohou být uložené hesla

### **Útok a bezpečnostní incident** (Attack, Sec. incident) - provádí útočník využitím zranitelnosti aktiva

- Způsobuje škodu na aktivech
- Generická kategorizace:
    - **Přírodní katastrofy** - hurikán, zemětřesení, požár, mohou zničit nezálohovaná data (zálohovat ve vzdálené lokalitě!)
    - **Externí útoky** - krádeže dat o kartách/lidech, hackery, profesionály
    - **Interní útoky** - např. web Wikileaks vznikl z interně zcizených dat
    - **Selhání, neúmyslné lidské chyby** - výpadek napětí, spojů, disků, vylití kávy do klávesnice, omylem zrušená data, ...

### **Riziko** (Risk) - pravděpodobnost, že se v daném zranitelném místě uplatní hrozba

- Velikost rizika je daná pravděpodobností provedení útoku a výší škody vzniklé útokem
- Uplatnění hrozby -
- možná něco dalšího?


---


## Prezentace 2

### **Riziko** - Reprezentace negativního dopadu využití zranitelnosti, tj. útoku, přičemž zohledňuje jak pravděpodobnost tak i škodní dopad útoku

**Rizika mohou plynout z**:
- Cílů a řešení podnikatelských procesů
- Nedokonalého vyhovění zákonným/smluvním závazkům
- Úrovně kvality návrhových, implementačních a provozních procedur aplikačních systémů

**Riziko se vyjadřuje**:
- V pravděpodobnostních pojmech (s jakou pravděpodobností se hrozba uplatní)
- V pojmech charakterizujících dopad hrozby (velikost škody způsobené útokem)
- Generické kombinované vyjádření úrovně rizika:
    **úroveň rizika = F(pravděpodobnost útoku) × F´(dopad útoku)**

**Zvládání rizik** - Rizika se zvládají volbou a uplatňováním vhodných opatření

