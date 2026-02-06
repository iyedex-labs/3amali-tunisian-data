# METADATA AND DATA STANDARDS
## VERSION 1.0 | IYEDEX DATA INITIATIVE

To ensure that the data collected is usable for training 3amAli and other LLMs, all submissions must adhere to the standardized formatting rules defined below.

---

## CORE JSON SCHEMA

Every data entry must be wrapped in a JSON object. We prioritize readability and consistency.

### 1. LINGUISTIC DATA (Chat, Q&A, Slang)
For folders under `01_chat_darja`, use this structure:

| FIELD | TYPE | DESCRIPTION |
| :--- | :--- | :--- |
| `instruction` | String | The prompt or question in Tunisian Darja. |
| `response` | String | The natural, accurate answer in Tunisian Darja. |
| `dialect_region` | String | Specific region if applicable (e.g., "Sfax", "Tunis", "South"). Use "Standard" otherwise. |
| `context` | String | The category of conversation (e.g., "Medical", "Travel", "SmallTalk"). |

### 2. FACTUAL & ENTERPRISE DATA
For folders under `04_enterprise` and `05_knowledge`, use this structure:

| FIELD | TYPE | DESCRIPTION |
| :--- | :--- | :--- |
| `subject` | String | The name of the entity, person, or event. |
| `fact_body` | String | A detailed, verified description or data points. |
| `source_url` | String | A link to the public record, news article, or official site. |
| `last_updated` | String | Date in YYYY-MM-DD format. |

---

## LANGUAGE REQUIREMENTS

1. **Strictly Tunisian**: Avoid "Literal Arabic" (Fousha) in the Darja folders. We want the AI to sound like a person from Tunisia, not a book.
2. **Script**: We prefer Arabic script for Darja. If "Tunizi" (Latin script with numbers like 3, 7, 9) is provided, it must be placed in a separate field named `latin_script`.
3. **No Hate Speech**: Any data containing offensive, discriminatory, or political hate speech will be rejected immediately.

---

## FILE NAMING CONVENTION

File names should be lowercase, using underscores instead of spaces.
* **Bad**: `My Data.json`
* **Good**: `sfax_history_facts_v1.json`
* **Good**: `street_slang_tunis_city.json`
