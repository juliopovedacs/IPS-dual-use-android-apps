# Global Survey of Android Dual-use Apps
## Abstract
Intimate partner violence (IPV) is a pervasive societal problem that affects millions of people around the world. IPV perpetrators increasingly weaponize digi- tal technologies like mobile applications (“apps”) to spy on, monitor, and harass victims. Surveillance-capable apps can have legitimate use cases, for example, locat- ing children, and are therefore easily available on vari- ous mobile app stores like the Google Play Store. Nev- ertheless, these applications are easily repurposed by abusers to track their victims. The problem of such dual-use apps in IPV is global. However, current un- derstanding of the ecosystem of such apps is limited to English-language apps, potentially limiting its rele- vance to non-English speaking IPV survivors across the world. In this paper, we study the prevalence of dual- use applications found in 15 languages and 27 coun- tries. We collected 51,868 unique apps in 2020 from the Google Play Store, using queries such as “track wife’s location.” Through a semi-manual analysis of a subset of these apps, we discovered 854 unique dual- use apps, and estimate that among the apps collected from Google Play, 3,988 are dual-use apps. We found no- table differences in app search results, suggested queries, and marketed capabilities of dual-use apps across differ- ent languages. For instance, we identified that 18% of dual-use apps do not have an English description, and 28% could not be found using English queries. Google Play (cursorily) blocks certain queries referring explic- itly to intimate partner surveillance (IPS) to discour- age potential abusers, but the blocking efficacy varies across languages. For example, we found that 80% of ex- plicit IPS queries for English are blocked, but none for Bengali, Chinese, Hindi, Malay, Thai, and Vietnamese. Thus, abusers fluent in those languages can evade such blocking with no effort.

## Main work
Our paper appears in PoPETS/PETS 2022; you may find the paper here (will be added soon). 

## Files included
1. `terms.csv`: 
2. `play_store.csv`: Contains all downloaded apps in 2020 and 2020. The file includes `appId`, `title`, `detected_language` (language of metadeta), `crawl_language` (qurey language used to obtain app), `crawl_year`, `ml_score`(classification score), `manual_label`, and `capabilities` (capabilities of flagged dual-use apps).
3. `flagged_apps_2020.csv`: All apps manually flagged in 2020
4. `flagged_apps_2022.csv`: All apps manually flagged in 2022
5. `chinese_stores.csv`: Contains all downloaded apps from the four Chinese app stores *Xiaomi*, *Baidu*, *Tencent*, and *Huawei*. The file includes `appId`, `title`, `manual_label`, and `capabilities` (capabilities of flagged dual-use apps).
6. `script.ipynb`: A script that compiles important results from the main analysis of 2020's crawl.
7. `play_store.db`: Contains `play_store.csv` as a table (The file will get removed after updating script.ipynb to use pandas instead of SQLite).

