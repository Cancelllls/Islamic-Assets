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

## Sources

- Hadith text: [sunnah.com](https://sunnah.com) via [hadith-json](https://github.com/AhmedBaset/hadith-json) and [Hadith-Data-Sets](https://github.com/irahardianto/Hadith-Data-Sets)
- Hadith grading: [meeAtif/hadith_datasets](https://huggingface.co/datasets/meeAtif/hadith_datasets) (MIT License)
- Musnad Ahmad: [irahardianto/Hadith-Data-Sets](https://github.com/irahardianto/Hadith-Data-Sets)

## License

Data sourced from public domain and MIT-licensed datasets. This repository is maintained as a CDN endpoint for the Aya app.
