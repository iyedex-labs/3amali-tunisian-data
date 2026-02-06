# 🇹🇳 TUNISIAN DATA HUB

## THE OPEN NATIONAL DATASET FOR ARTIFICIAL INTELLIGENCE

Tunisian Data Hub is a massive, high-granularity digital library created and licensed by **IyedeX**. This repository is the foundational training ground for **3amAli** and any future Tunisian AI models. It is designed to be the "Wikipedia of Tunisian Data"—open for the community to enrich, refine, and expand.

---

## PROJECT CORE ARCHITECTURE

The structure is optimized for **Large Language Models (LLMs)**. By separating data into many specific folders, we allow AI to learn context, humor, professional tone, and factual accuracy independently.

| LAYER | FOCUS | OBJECTIVE |
| --- | --- | --- |
| **01 LINGUISTICS** | Darja & Chat | Natural flow and conversational intelligence |
| **02 ENTERTAINMENT** | Jokes & Media | Sarcasm, humor, and cultural wit |
| **03 WISDOM** | Proverbs & Quotes | Traditional values and metaphorical reasoning |
| **04 BUSINESS** | Enterprise & Law | Professional assistance and economic logic |
| **05 FACTUAL** | History & Places | Grounded truth and national knowledge |

---

## FILE STRUCTURE

This structure is designed for "Ease of Entry." Developers can quickly find where their data belongs.

```text
root/
├── data/
│   ├── 01_chat_darja/
│   │   ├── q_a_casual/              | Daily "Question & Response" pairs
│   │   ├── q_a_technical/           | Tech support questions in Darja
│   │   ├── street_interactions/     | Raw dialogues from real life
│   │   └── regional_slang/          | Specific words (Sfax, North, South)
│   ├── 02_humor_nokat/
│   │   ├── nokat_short/             | One-liner jokes
│   │   ├── nokat_long/              | Stories and satirical tales
│   │   └── memes_text/              | Common Tunisian social media text
│   ├── 03_wisdom_amthal/
│   │   ├── amthal_sha3biya/         | Traditional proverbs
│   │   ├── aqwal_famous/            | Famous quotes from Tunisians
│   │   └── hikma_wisdom/            | General life advice in Darja
│   ├── 04_enterprise_economy/
│   │   ├── company_profiles/        | Public data on Tunisian firms
│   │   ├── startup_data/            | Tech ecosystem info
│   │   ├── jort_laws/               | Simplified legal texts
│   │   └── banking_finance/         | Public reports and tax info
│   ├── 05_knowledge_facts/
│   │   ├── history_timeline/        | Dates and historical events
│   │   ├── personality_bios/        | Biographies of Tunisian figures
│   │   ├── geography_cities/        | Data on every Mutamadiya/Imada
│   │   └── archaeology_sites/       | Facts about ruins and monuments
│   └── 06_lifestyle_media/
│       ├── gastronomy_recipes/      | Ingredients and cooking steps
│       ├── tv_scripts/              | Dialogue from Tunisian series
│       └── music_lyrics/            | Lyrics and artist backgrounds
└── docs/
    ├── metadata_standards.md
    └── contribution_guide.md

```

---

## DATA FORMATS

To make this dataset ready for training (GPT, Llama, 3amAli), please use the following formats:

### For Chat (Q&A)

**File: `data/01_chat_darja/q_a_casual/sample.json**`

```json
{
  "instruction": "كيفاش انجم نمشي من تونس لسوسة بالترينو؟",
  "response": "تمشي لمحطة برشلونة، تقص تذكرة في ترينو القلعة الساحلية، والرحلات موجودة تقريبا كل ساعة.",
  "context": "transportation",
  "verified": true
}

```

### For Jokes/Proverbs

**File: `data/02_humor_nokat/nokat_short/sample.json**`

```json
{
  "text": "مرة واحد مشا يخطب، قالو بو الطفلة شتعمل في حياتك؟...",
  "type": "classic_humor",
  "rating": "family_friendly"
}

```

---

## HOW TO CONTRIBUTE (EASY STEPS)

You don't need to be an AI expert to help. Just follow these steps:

1. **FORK**: Click the 'Fork' button at the top of this repo.
2. **PICK A FOLDER**: Decide what you want to add (e.g., Jokes in `02_humor_nokat`).
3. **ADD DATA**: Create a new `.json` file. Name it clearly (e.g., `jokes_by_ahmed.json`).
4. **FORMAT**: Use the JSON structure shown above.
5. **PULL REQUEST**: Submit your changes for review.

---

## GOVERNANCE & LICENCE

* **Created By**: **IyedeX**
* **Purpose**: Training **3amAli** and empowering the Tunisian AI ecosystem.
* **Licence**: **Creative Commons Attribution 4.0 International (CC BY 4.0)**.
* *You are free to share and adapt the data, but you must give credit to IyedeX and the community contributors.*



---

## COMMUNITY SUPPORT

For complex data structures or big data dumps, please open an **Issue** or contact the **IyedeX** team directly. Let's build the largest open brain for Tunisia.
