# Islamic Assets

Open Islamic data files for the [Aya Islamic App](https://github.com/Cancelllls/Aya) — served via [jsDelivr](https://www.jsdelivr.com/) CDN.

## Contents

### Hadith Collections (13 books, ~75,000 hadiths)

| Book | Arabic | English | Hadiths |
|------|--------|---------|---------|
| Sahih al-Bukhari | ✓ | ✓ | 7,277 |
| Sahih Muslim | ✓ | ✓ | 7,367 |
| Sunan Abu Dawud | ✓ | ✓ | 5,276 |
| Jami' at-Tirmidhi | ✓ | ✓ | 4,053 |
| Sunan an-Nasa'i | ✓ | ✓ | 5,685 |
| Sunan Ibn Majah | ✓ | ✓ | 4,079 |
| Musnad Ahmad | ✓ | — | 26,363 |
| Muwatta Malik | ✓ | ✓ | 1,985 |
| Riyad as-Salihin | ✓ | ✓ | 1,896 |
| Al-Adab Al-Mufrad | ✓ | ✓ | 1,326 |
| Bulugh al-Maram | ✓ | ✓ | 1,767 |
| Mishkat al-Masabih | ✓ | ✓ | 4,428 |
| Shama'il Muhammadiyah | ✓ | ✓ | 402 |

### Hadith Grading

`hadith/grades.json` — offline grading for 4 books (Tirmidhi, Abu Dawud, Nasai, Ibn Majah) sourced from the [HuggingFace Hadith Dataset](https://huggingface.co/datasets/meeAtif/hadith_datasets).

## CDN Usage

```
https://cdn.jsdelivr.net/gh/Cancelllls/Islamic-Assets@main/hadith/{lang}-{book}.json
```

Example:
```
https://cdn.jsdelivr.net/gh/Cancelllls/Islamic-Assets@main/hadith/ara-bukhari.json
```


### Quran (Hafs + 10 Qira'at)

| File | Recitation | Size |
|------|-----------|------|
| `quran_hafs.json` | Hafs 'an 'Asim (standard) | 14 MB |
| `warsh.json` | Warsh 'an Nafi' | 2.7 MB |
| `qaloon.json` | Qaloon 'an Nafi' | 3.0 MB |
| `bazzi.json` | Al-Bazzi 'an Ibn Kathir | 3.0 MB |
| `qunbul.json` | Qunbul 'an Ibn Kathir | 3.0 MB |
| `duri.json` | Al-Duri 'an Abu 'Amr | 3.0 MB |
| `susi.json` | Al-Susi 'an Abu 'Amr | 3.0 MB |
| `hisham.json` | Hisham 'an Ibn 'Amir | 3.0 MB |
| `ibn-dhakwan.json` | Ibn Dhakwan 'an Ibn 'Amir | 3.0 MB |
| `shuba.json` | Shu'ba 'an 'Asim | 3.0 MB |
| `surahs.json` | Surah metadata | 28 KB |

CDN: `https://cdn.jsdelivr.net/gh/Cancelllls/Islamic-Assets@main/quran/{file}.json`


### Hadith Sharh (Classical Explanations)

Per-book files in `sharh/` directory — JSON, each under 27MB:

| Book | File | Hadiths | Source | Size |
|------|------|---------|--------|------|
| Bukhari | `sharh/sharh_bukhari.json` | 5,483 / 7,277 | Fath al-Bari | 26.9 MB |
| Abu Dawud | `sharh/sharh_abudawud.json` | 4,270 / 5,276 | Awn al-Ma'bud | 18.0 MB |
| Nasai | `sharh/sharh_nasai.json` | 2,108 / 5,685 | Hashiya al-Sindi | 4.2 MB |
| Tirmidhi | `sharh/sharh_tirmidhi.json` | 1,131 / 4,053 | al-Urf al-Shadhi | 2.5 MB |
| Muslim | `sharh/sharh_muslim.json` | 574 / 7,368 | Sharh al-Nawawi | 3.0 MB |
| **Total** | | **13,566** | | **54.6 MB** |

CDN example:
```
https://cdn.jsdelivr.net/gh/Cancelllls/Islamic-Assets@main/sharh/sharh_bukhari.json
```

Sources: OpenITI Corpus (Zenodo) + Maktaba Shamela (HuggingFace)

## Sources

- Quran text: Standard Uthmani script (Hafs) + 10 Qira'at variants


### Hadith Sharh (Classical Explanations)

Per-book files in `sharh/` directory — JSON, each under 27MB:

| Book | File | Hadiths | Source | Size |
|------|------|---------|--------|------|
| Bukhari | `sharh/sharh_bukhari.json` | 5,483 / 7,277 | Fath al-Bari | 26.9 MB |
| Abu Dawud | `sharh/sharh_abudawud.json` | 4,270 / 5,276 | Awn al-Ma'bud | 18.0 MB |
| Nasai | `sharh/sharh_nasai.json` | 2,108 / 5,685 | Hashiya al-Sindi | 4.2 MB |
| Tirmidhi | `sharh/sharh_tirmidhi.json` | 1,131 / 4,053 | al-Urf al-Shadhi | 2.5 MB |
| Muslim | `sharh/sharh_muslim.json` | 574 / 7,368 | Sharh al-Nawawi | 3.0 MB |
| **Total** | | **13,566** | | **54.6 MB** |

CDN example:
```
https://cdn.jsdelivr.net/gh/Cancelllls/Islamic-Assets@main/sharh/sharh_bukhari.json
```

Sources: OpenITI Corpus (Zenodo) + Maktaba Shamela (HuggingFace)

## Sources

- Hadith text: [sunnah.com](https://sunnah.com) via [hadith-json](https://github.com/AhmedBaset/hadith-json) and [Hadith-Data-Sets](https://github.com/irahardianto/Hadith-Data-Sets)
- Hadith grading: [meeAtif/hadith_datasets](https://huggingface.co/datasets/meeAtif/hadith_datasets) (MIT License)
- Musnad Ahmad: [irahardianto/Hadith-Data-Sets](https://github.com/irahardianto/Hadith-Data-Sets)

## License

Data sourced from public domain and MIT-licensed datasets. This repository is maintained as a CDN endpoint for the Aya app.
