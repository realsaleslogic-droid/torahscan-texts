# TorahScan texts

The texts the TorahScan apps show: every daf-side of the Talmud Bavli, every
chapter of Tanakh and every aliyah of the Torah, and Rashi on each, as one
gzipped JSON file per section (`text/` and `rashi/`). They were fetched once
from [Sefaria](https://www.sefaria.org)'s public API, so the apps don't
depend on Sefaria being reachable. `missing.txt` lists the sections Sefaria
has no text for.

Made by `native/build-texts.mts` in the TorahScan app's repository; read by
`src/lib/texts.ts` there.

## The texts and their licenses

Texts are provided by [Sefaria](https://www.sefaria.org) under these licenses.
Licenses marked NC permit non-commercial use only, which is how TorahScan uses
them (it is free, with no ads).

- **Talmud, Aramaic and English:** The William Davidson Edition, Koren Noé
  Talmud, with commentary by Rabbi Adin Even-Israel Steinsaltz —
  [CC BY-NC](https://creativecommons.org/licenses/by-nc/4.0/).
- **Tanakh, Hebrew:** Miqra according to the Masorah —
  [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/).
- **Tanakh, English:** The JPS Tanakh: Gender-Sensitive Edition, © Jewish
  Publication Society — [CC BY-NC](https://creativecommons.org/licenses/by-nc/4.0/).
- **Rashi on the Talmud:** Vilna Edition, public domain; English, where shown,
  the Sefaria Community Translation, CC0.
- **Rashi on the Torah:** Pentateuch with Rashi's commentary by M. Rosenbaum
  and A. M. Silbermann (1929–1934), Hebrew and English, public domain.
- **Rashi on Nevi'im and Kesuvim:** Hebrew, Vocalized Edition, CC0; English,
  The Judaica Press complete Tanach with Rashi, translated by A. J. Rosenberg —
  [CC BY](https://creativecommons.org/licenses/by/4.0/).

Each file keeps its text exactly as Sefaria gave it, in a different
arrangement (by section). Shared under the same licenses as above.
