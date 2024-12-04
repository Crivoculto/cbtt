# Anatomia de um item
##  Raridades
| Comum | Mágico | Raro | Único |
|:---|:---|:---|:---|
| ![Comum](img/itemComum.png) | ![Mágico](img/itemMagico.png) | ![Raro](img/itemRaro.png) | ![Único](img/itemUnico.png)|

## Mods / Affixes
Mods, modificadores ou `Affixes` são divididos em duas categorias, `Prefix` e `Suffix`. Os modificadores `Prefix` não podem aparecer como `Suffix` e vice-versa.

<p align="center">
  <img src="./img/itemRaroMarcado.png" width="500">
</p>



A raridade do item define a quantos `affixes` um item pode ter.

| Comum | Mágico | Raro |
|:---|:---|:---|
| 0 Affixes | 1-2 Affixes | 3-6 Affixes |

## Encantamentos ou implícitos
Os implícitos são mods especiais que vêm embutidos em certos itens, separados dos mods prefixos e sufixos. Esses mods não ocupam espaço nas modificações mágicas, raras ou únicas do item, e são sempre fixos no tipo e no número de mods possíveis para aquele item específico.

⚠️ Os implícitos não podem ser craftados.

<p align="center">
  <img src="./img/itemRaroImplicit.png" width="500">
</p>

## Qualidade
Influência o status principal do item. Ex.: Dano em armas e defesa / dodge em armaduras.

## Soquetes
Espaço onde pode ser colocado uma `Rune` ou `Soul Core`.
- Não podem ser removidos.
- Máximo de 2 `socket` em armas de duas mãos e peitorais.
- Máximo de 1 `socket` em armas de uma mão e demais peças de armadura.

💎 `Soul Core` oferece buffs diferentes de `Rune` mas funciona da mesma forma. Dropam do `Trial of the Chaos God`, atividade do end-game.

# Mecânicas de crafting básico

## Currency / Itens de crafting
| Img | Item |  Efeito |
|:---|:---|:---|
| Chaos Orb | ![Chaos Orb](img/chaosOrb.webp) | Remove um modificador aleatório e adiciona um modificador aleatório. |
| Divine Orb | ![Divine Orb](img/divineOrb.webp) | Randomiza os valores numéricos de um item. |
| Exalted Orb | ![Exalted Orb](img/exaltedOrb.webp) | Adiciona um modificador aleatório a um <ins>item raro</ins>. |
| Orb of Alchemy | ![Orb of Alchemy](img/orbOfAlchemy.webp) | Atualiza um item <ins>normal</ins> para um item raro com 4 modificadores. |
| Orb of Annulment | ![Orb of Annulment](img/orbOfAnnulment.webp) | Remove um modificador aleatório. |
| Orb of Augmentation | ![Orb of Augmentation](img/orbOfAugmentation.webp) | Adiciona um modificador aleatório a um item <ins>mágico</ins> |
| Orb of Chance | ![Orb of Chance](img/orbOfChance.webp) | Transforma um item <ins>normal</ins> em um item mágico, raro ou único de forma aleatória. |
| Orb of Transmutation | ![Orb of Transmutation](img/orbOfTransmutation.webp) | Transforma um item <ins>normal</ins> em um item mágico com um modificador |
| Regal Orb | ![Regal Orb](img/regalOrb.webp) | Transforma um item <ins>normal</ins> em um item raro |
| Vaal Orb | ![Vaal Orb](img/vaalOrb.webp) | Modifica o item de forma imprevisível e única. Adiciona [corrupção](#vaal-orb) o item. |



## Progressão simples

```mermaid
flowchart TD
    Normal["Normal (0 mods)"] -->| Orb of Transmutation | Magic["Magic (1 mod)"]
    Magic -->| Orb of Augmentation <br>+1 Modificador | MagicPlus["Mágico (2 mods)"]
    MagicPlus -->| Orb of Annulment <br>-1 Modificador | Magic["Mágico (1 mod)"]
    Normal["Normal (0 mods)"] -->| Orb of Alchemy | RarePlus["Raro (4 mods)"]
    Magic -->| Orb of Alchemy | Rare["Raro (3 mods)"]
    Rare -->| Exalted Orb <br>+1 Modificador | RarePlus["Raro (4 mods)"]
    RarePlus -->| Exalted Orb <br>+1 Modificador | RareMega["Raro (5 mods)"]
    RareMega -->| Exalted Orb <br>+1 Modificador | RareUltra["Raro (6 mods)"]

    style Normal fill:#aeb6bf,stroke:#1c2833,stroke-width:3px, font-size:16px, color:#1c2833
    style Magic fill:#85c1e9,stroke:#1c2833,stroke-width:3px, font-size:16px, color:#1c2833
    style MagicPlus fill:#85c1e9,stroke:#1c2833,stroke-width:3px, font-size:16px, color:#1c2833
    style Rare fill:#f7dc6f,stroke:#1c2833,stroke-width:3px, font-size:16px, color:#1c2833
    style RarePlus fill:#f7dc6f,stroke:#1c2833,stroke-width:3px, font-size:16px, color:#1c2833
    style RareMega fill:#f7dc6f,stroke:#1c2833,stroke-width:3px, font-size:16px, color:#1c2833
    style RareUltra fill:#f7dc6f,stroke:#1c2833,stroke-width:3px, font-size:16px, color:#1c2833

    linkStyle 0 stroke:#16a085,stroke-width:4px, color:#ffffff
    linkStyle 1 stroke:#16a085,stroke-width:4px, color:#ffffff
    linkStyle 2 stroke:#c0392b,stroke-width:4px, color:#ffffff
    linkStyle 3 stroke:#16a085,stroke-width:4px, color:#ffffff
    linkStyle 4 stroke:#16a085,stroke-width:4px, color:#ffffff
    linkStyle 5 stroke:#16a085,stroke-width:4px, color:#ffffff
    linkStyle 6 stroke:#16a085,stroke-width:4px, color:#ffffff
    linkStyle 7 stroke:#16a085,stroke-width:4px, color:#ffffff
```

loop HealthCheck
    John->>John: Fight against hypochondria
end

## Chaos Orb
## Vaal Orb

# Crafting no end-game
## Essencias
## 
