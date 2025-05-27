graph TD
    subgraph Salle de Conférence
        MacMini[Mac mini M4] -->|USB-C| HubUSB[Hub USB-C / Thunderbolt]
        MacMini -->|HDMI| TV55[Téléviseur 55" Continental Edison]
        MacMini -->|HDMI| Moniteur22[Moniteur 22"]

        HubUSB -->|USB-C| ATEM[Blackmagic ATEM Mini Pro ISO]
        HubUSB -->|USB| AudioInterface[Interface Audio USB]
        HubUSB -->|USB-C| Kandao[Kandao Meeting Pro 360°]
        HubUSB -->|USB| ClavierSouris[Clavier & Souris Apple]

        ATEM -->|HDMI (Programme Out)| TV55
        ATEM -->|HDMI (Programme Out)| Moniteur22

        SystemeConferenceTOA[Système Conférence TOA TS-770] -->|Audio Out (RCA/Euroblock)| AudioInterface
        AudioInterface -->|Audio In (RCA/Euroblock)| SystemeConferenceTOA

        Kandao -->|Audio & Video In/Out (USB)| ATEM
        Kandao -->|Audio & Video In/Out (USB)| MacMini

        OrdinateurPortableInv[Ordinateur Portable Invité (Optionnel)] -->|HDMI| ATEM
    end

    style MacMini fill:#E6F0FF,stroke:#3366CC,stroke-width:2px
    style TV55 fill:#FFDDC1,stroke:#FF9933,stroke-width:2px
    style Moniteur22 fill:#FFDDC1,stroke:#FF9933,stroke-width:2px
    style HubUSB fill:#F0F0F0,stroke:#666666,stroke-width:2px
    style ATEM fill:#D1FFD1,stroke:#009900,stroke-width:2px
    style AudioInterface fill:#D1FFD1,stroke:#009900,stroke-width:2px
    style Kandao fill:#E0E0FF,stroke:#6666FF,stroke-width:2px
    style SystemeConferenceTOA fill:#FFE0E0,stroke:#CC3333,stroke-width:2px
    style ClavierSouris fill:#E6F0FF,stroke:#3366CC,stroke-width:2px
    style OrdinateurPortableInv fill:#F0F0F0,stroke:#666666,stroke-width:1px,stroke-dasharray: 5 5

    linkStyle 0 stroke-width:2px,stroke:#3366CC;
    linkStyle 1 stroke-width:2px,stroke:#FF9933;
    linkStyle 2 stroke-width:2px,stroke:#FF9933;
    linkStyle 3 stroke-width:2px,stroke:#009900;
    linkStyle 4 stroke-width:2px,stroke:#009900;
    linkStyle 5 stroke-width:2px,stroke:#6666FF;
    linkStyle 6 stroke-width:2px,stroke:#3366CC;
    linkStyle 7 stroke-width:2px,stroke:#FF9933;
    linkStyle 8 stroke-width:2px,stroke:#FF9933;
    linkStyle 9 stroke-width:2px,stroke:#CC3333;
    linkStyle 10 stroke-width:2px,stroke:#009900;
    linkStyle 11 stroke-width:2px,stroke:#6666FF;
    linkStyle 12 stroke-width:2px,stroke:#3366CC;
    linkStyle 13 stroke-width:2px,stroke:#666666;
