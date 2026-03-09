| Nome colonna             | Tipo di dato                                                                                                 | Attributi                             | Indice      |
| ------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------- | ----------- |
| id                       | BIGINT                                                                                                       | NOT NULL, UNIQUE, AUTOIMPLEMENT       | PRIMARY KEY |
| numero_targa             | CHAR(7)                                                                                                      | NULL,                                 |             |
| Marca                    | VARCHAR(50)                                                                                                  | NOT NULL, DEFAULT(VEICOLO SPECIALE)   | INDEX       |
| modello                  | VARCHAR(50)                                                                                                  | NULL                                  | INDEX       |
| motore                   | ENUM("ASPIRATO", "TURBO")                                                                                    | NULL                                  |             |
| cambio                   | ENUM("MANUALE", "AUTOMATICO","DOPPIA FRIZIONE(dct, dsg, tct), "ROBOTIZZATO", "SEQUENZIALE", "SPECIALE")      | NOT NULL,                             | INDEX       |
| numero_marce             | TINYINT                                                                                                      | NULL, UNSIGNED                        |             |
| retro?                   | BOOLEAN                                                                                                      | NULL                                  |             |
| numero_cavalli           | SMALLINT                                                                                                     | NULL, UNSIGNED                        |             |
| alimentazione            | ENUM("BENZINA", "GASOLIO", "GAS", "ELETTRICA", "ZOLFO", "IDROGENO", "A PIOMBO")                              | NOT NULL                              | INDEX       |
| truccata                 | BOOLEAN                                                                                                      | DEFAULT(DA VERIFICARE)                |             |
| accelerazione_da_0_a_100 | FLOAT(6,3)                                                                                                   | NULL                                  |             |
| velocità_massima         | FLOAT(5,2)                                                                                                   | NULL                                  |             |
| sponsorizzata            | BOOLEAN                                                                                                      | NULL                                  |             |
| nome_sponsor             | VARCHAR(20)                                                                                                  | NULL                                  |             |
| anno_fabbricazione       | YEAR                                                                                                         | NULL                                  |             |
| anno_immatricolazione    | YEAR                                                                                                         | NOT NULL DEFAULT("NON ANCORA IMMAT.") |             |
| chilometri_percorsi      | MEDIUMINT                                                                                                    | NOT NULL                              |             |
| tagliandi_regolari       | BOOLEAN                                                                                                      | DEFAULT(NON SPECIFICATO)              |             |
| ultimo_tagliando         | DATE                                                                                                         | NOT NULL                              |             |
| revisione                | BOOLEAN                                                                                                      | NOT NULL                              |             |
| ultima_revisione         | DATE                                                                                                         | NOT NULL                              |             |
| incidenti                | BOOLEAN                                                                                                      | NOT NULL                              |             |
| stato_scocca             | ENUM("ECCELLENTE", "COME NUOVO", "BUONO", "AMMACCATA", "ARRUGGINITA", "DA RIFARE")                           | NULL                                  |             |
| stato_ciclistico         | ENUM("ECCELLENTE", "COME NUOVO", "APPENA REVISIONATO", "DA REVISIONARE", "PARZIALMENTE GUASTO", "DA RIFARE") | NULL                                  |             |
| numero_proprietari       | TINYINT                                                                                                      | UNSIGNED                              |             |
| descrizione_veicolo      | TEXT                                                                                                         | NULL                                  |             |
| possibilità_di_leasing   | BOOLEAN                                                                                                      | NULL                                  |             |
| prezzo_stimato           | INT                                                                                                          | NULL                                  |             |
| prezzo_trattabile        | BOOLEAN                                                                                                      | NULL                                  |             |
| incentivata              | BOOLEAN                                                                                                      | NOT NULL                              |             |
