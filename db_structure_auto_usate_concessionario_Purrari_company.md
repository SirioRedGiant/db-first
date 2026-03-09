| Nome colonna             | Tipo di dato                                                                                                 | Attributi                           | Indice      |
| ------------------------ | ------------------------------------------------------------------------------------------------------------ | ----------------------------------- | ----------- |
| id                       | BIGINT                                                                                                       | NOT NULL, UNIQUE, AUTOIMPLEMENT     | PRIMARY KEY |
| numero_targa             | CHAR(7)                                                                                                      | NULL,                               |             |
| Marca                    | VARCHAR(50)                                                                                                  | NOT NULL, DEFAULT(VEICOLO SPECIALE) | INDEX       |
| modello                  | VARCHAR(50)                                                                                                  | NULL                                | INDEX       |
| motore                   | ENUM("ASPIRATO", "TURBO")                                                                                    |                                     |             |
| cambio                   | ENUM("MANUALE", "AUTOMATICO","DOPPIA FRIZIONE(dct, dsg, tct), "ROBOTIZZATO", "SEQUENZIALE", "SPECIALE")      | NOT NULL,                           | INDEX       |
| numero_marce             | TINYINT                                                                                                      | NULL, UNSIGNED                      |             |
| retro?                   | BOOLEAN                                                                                                      | NULL                                |             |
| numero_cavalli           | SMALLINT                                                                                                     | NULL, UNSIGNED                      |             |
| alimentazione            | ENUM("BENZINA", "GASOLIO", "GAS", "ELETTRICA", "ZOLFO", "IDROGENO", "A PIOMBO")                              |                                     | INDEX       |
| truccata                 | BOOLEAN                                                                                                      |                                     |             |
| accelerazione_da_0_a_100 | FLOAT(6,3)                                                                                                   | NULL                                |             |
| velocità_massima         | FLOAT(5,2)                                                                                                   | NULL                                |             |
| sponsorizzata            | BOOLEAN                                                                                                      | NULL                                |             |
| nome_sponsor             | VARCHAR(20)                                                                                                  |                                     |             |
| anno_fabbricazione       | YEAR                                                                                                         |                                     |             |
| anno_immatricolazione    | YEAR                                                                                                         |                                     |             |
| chilometri_percorsi      | MEDIUMINT                                                                                                    |                                     |             |
| tagliandi_regolari       | BOOLEAN                                                                                                      |                                     |             |
| ultimo_tagliando         | DATE                                                                                                         |                                     |             |
| revisione                | BOOLEAN                                                                                                      |                                     |             |
| ultima_revisione         | DATE                                                                                                         |                                     |             |
| incidenti                | BOOLEAN                                                                                                      |                                     |             |
| stato_scocca             | ENUM("ECCELLENTE", "COME NUOVO", "BUONO", "AMMACCATA", "ARRUGGINITA", "DA RIFARE")                           |                                     |             |
| stato_ciclistico         | ENUM("ECCELLENTE", "COME NUOVO", "APPENA REVISIONATO", "DA REVISIONARE", "PARZIALMENTE GUASTO", "DA RIFARE") |                                     |             |
| numero_proprietari       | TINYINT                                                                                                      |                                     |             |
| descrizione_veicolo      | TEXT                                                                                                         |                                     |             |
| possibilità_di_leasing   | BOOLEAN                                                                                                      |                                     |             |
| prezzo_stimato           | INT                                                                                                          |                                     |             |
| prezzo_trattabile        | BOOLEAN                                                                                                      |                                     |             |
| incentivata              | BOOLEAN                                                                                                      |                                     |             |
