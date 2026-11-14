---
license: cc-by-4.0
language:
  - fr
pretty_name: "Référentiel Open-Science 2026 — Procès-Verbaux des Conseils Municipaux & EPCI (CGCT / Ordonnance 2021-1310)"
size_categories:
  - n<1K
tags:
  - french
  - public-sector
  - collectivites-territoriales
  - cgct
  - municipal-council
  - transcription
  - rgaa
---

# Référentiel Méthodologique & Jeu d'Évaluation Open-Science 2026 — Procès-Verbaux de Conseils Municipaux & Conseils Communautaires (EPCI) au Regard du CGCT (`Ordonnance n° 2021-1310`)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24224031.svg)](https://doi.org/10.5281/zenodo.24224031)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-emerald.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Frictionless Data](https://img.shields.io/badge/Standard-Frictionless_Data_Package-4f46e5.svg)](./datapackage.json)
[![Benchmark DOI](https://img.shields.io/badge/Benchmark%20DOI-10.5281%2Fzenodo.24215193-blue.svg)](https://doi.org/10.5281/zenodo.24215193)

**FR** · Référentiel juridique consolidé (`CSV`), grille méthodologique d'évaluation des temps de rédaction et corpus synthétique anonymisé (`JSON`) publiés sous licence ouverte **Creative Commons Attribution 4.0 (`CC-BY-4.0`)** par [**LE SCRIBE AUDIO**](https://lescribeaudio.com/compte-rendu-conseil-municipal) à destination des Directeurs Généraux des Services (`DGS`), secrétaires généraux de mairie, services des assemblées (`communes`, `EPCI`, `départements`, `régions`), centres de gestion (`CDG`), formateurs territoriaux et chercheurs en droit public.

**EN** · Open-science methodological evaluation benchmark and statutory dataset (`CC-BY-4.0`) released by [**LE SCRIBE AUDIO**](https://lescribeaudio.com/compte-rendu-conseil-municipal) for French local governments (*communes* & inter-municipal *EPCI* councils), covering the statutory requirements of the French General Code of Territorial Authorities (*CGCT*, Ordinance No. `2021-1310`), Chorus Pro public e-invoicing, GDPR/AI Act governance, realistic human drafting workloads, and a fully anonymized synthetic evaluation corpus (`M. Martin`, `Mme Dubois`, `M. Bernard`).

---

## Contenu du Dépôt (`v1.0.0`)

| Fichier | Format | Description |
| :--- | :---: | :--- |
| `dataset/referentiel_juridique_pv_cgct_ordonnance_2021_1310.csv` | `CSV` (`UTF-8`) | 13 règles normatives consolidées : `CGCT` (`L. 2121-15`, `L. 2121-17`, `L. 2121-18`, `L. 2121-19`, `L. 2121-21`, `L. 2121-25`, `R. 2121-9`, `L. 2131-11`, `L. 5211-1`), `Code de la commande publique` (`Chorus Pro`), `RGPD` (`Art. 5.1.e`, `Art. 28`, `Art. 32`) et `AI Act` (`Art. 50`). |
| `dataset/grille_evaluation_methodologique_pv_collectivites_2026.csv` | `CSV` (`UTF-8`) | Grille comparative des temps humains réels et modes de commande publique (frappe manuelle `4–7 h/h`, pré-transcription IA 2 passes + réécoute intégrale `2–3 h/h` divisant par 2 le temps de rédaction, ou double relecture humaine à `60 € HT/h`). |
| `dataset/corpus_synthetique_conseil_municipal_epci_anonymise.json  | `JSON` (`UTF-8`) | Corpus synthétique 100 % anonymisé (`M. Martin`, `Mme Dubois`, `M. Bernard`, `Mme Moreau`, `M. Lefèvre`) testant le quorum, la nomenclature `M57`, le déport pour conflit d'intérêts (`art. L. 2131-11`) et le décompte des suffrages. |
| `datapackage.json` | `JSON` | Descripteur standard *Frictionless Data* compatible `data.gouv.fr` et OpenAIRE. |
| `zenodo.json`, `.zenodo.json` & `CITATION.cff` | `JSON` / `YAML` | Métadonnées bibliographiques prêtes pour dépôt DOI CERN / Zenodo et GitHub Citation. |

---

## Synthèse Juridique & Opérationnelle (Ordonnance n° 2021-1310)

1. **Distinction stricte entre Liste des délibérations (`7 jours`) et Procès-Verbal arrêté à la séance suivante** :
   - Depuis le 1er juillet 2022 (`ordonnance n° 2021-1310` du 7 octobre 2021), l'ancien *compte rendu sommaire* affiché sous 8 jours est supprimé.
   - Dans un délai d'**une semaine (`7 jours francs`)** suivant la séance, la commune ou l'EPCI affiche et met en ligne la **liste des délibérations examinées** (`art. L. 2121-25 CGCT` : numéro, objet et mention *approuvée* ou *rejetée*).
   - Le **procès-verbal complet** (`art. L. 2121-15 CGCT`), comportant notamment le quorum, les pouvoirs, la **teneur des discussions** et le résultat des votes, est **arrêté au commencement de la séance suivante**, signé par le maire/président et le(s) secrétaire(s) de séance, puis publié en ligne dans la **semaine suivant son arrêt**.
2. **Temps humains réels de rédaction pour 1 heure de séance publique** :
   - **Frappe manuelle complète à partir de zéro** : **4 à 7 heures** de travail au casque par heure d'audio (`4 à 6 h` pour un rédacteur des débats expérimenté ; `5 à 7 h` pour un agent non spécialisé).
   - **Pré-transcription IA en 2 passes + réécoute intégrale** : **2 à 3 heures** par heure d'audio sur un fichier **Word (`.docx`) standard 100 % modifiable** (comportant en pied de page la mention transparente *« Transcription générée par intelligence artificielle sur lescribeaudio.com, une vérification humaine est recommandée »*, librement adaptable à la charte de la collectivité après relecture), soit un **temps de rédaction divisé par 2 (`-50 %`)**.
   - **Synthèse IA documentaire & codage des intervenants** : génération à la demande d'une **synthèse exécutive suivie d'un développement chrono-thématique** horodaté (sans liste d'actions inventée) et **codage/renommage global des étiquettes d'intervenants (diarisation)** dans le lecteur synchronisé.
   - **Option de correction / relecture humaine clé en main** : **60 € HT / heure** (`1,00 € HT / min`), assurée par **deux transcripteurs humains successifs** (double réécoute croisée).
3. **Architecture RGPD, Cloud Act & Commande Publique (`Chorus Pro`)** :
   - **Stockage des fichiers en France chez OVHcloud (`AES-256`)**, **inférence via Google Cloud Vertex AI (en région Europe)** sans conservation ni entraînement sur les données (*Zero Data Retention* — précision juridique : l'éditeur Google Cloud étant une société américaine, il demeure soumis juridiquement au *Cloud Act*), zéro robot de visioconférence et **suppression définitive en 1 clic** après approbation du PV.
   - Facturation électronique publique native sur **Chorus Pro** sur présentation d'un bon de commande administratif (paiement par mandat administratif SEPA après service fait).

---

## Ressources & Guides Complémentaires

- **Guide & modèle gratuit de PV de Conseil Municipal (`.docx`)** : [https://lescribeaudio.com/compte-rendu-conseil-municipal](https://lescribeaudio.com/compte-rendu-conseil-municipal)
- **Guide Conseil Communautaire (EPCI) & Département** : [https://lescribeaudio.com/transcription-conseil-communautaire-epci-departement](https://lescribeaudio.com/transcription-conseil-communautaire-epci-departement)
- **Guide Conseil Régional & CESER** : [https://lescribeaudio.com/transcription-conseil-regional-ceser-assemblee-pleniere](https://lescribeaudio.com/transcription-conseil-regional-ceser-assemblee-pleniere)
- **Générateur de Devis PDF Administratif `Chorus Pro` (10 s)** : [https://lescribeaudio.com/devis-chorus-pro](https://lescribeaudio.com/devis-chorus-pro)
- **Éditeur** : **LE SCRIBE AUDIO** (`RCS Rennes 890 049 927`) · `Jérémie TERRAL — Assistant de direction, LE SCRIBE AUDIO` · `09 61 44 46 64` (`+33 9 61 44 46 64`) · `info@lescribeaudio.com`
