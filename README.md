# Základy umělé inteligence (4IT_GRS1_25-26)

Aktualizováno: 17. září 2025

Tento repozitář obsahuje výukové materiály pro roční kurz Základy umělé inteligence (cca 60 hodin) v češtině. Materiály jsou primárně ve formě Jupyter/Colab sešitů (souborů `.ipynb`) a jsou doplněny sylabem a odkazy na oficiální dokumentaci všech použitých knihoven.

## Rychlý start

- Nejrychlejší (bez instalace):
  - Otevři libovolný sešit `AI_Zaklady_Hodina_XX.ipynb` v Google Colab (pravým tlačítkem → "Open in Colab" nebo nahraj přes [colab.research.google.com](https://colab.research.google.com)).

- Lokálně na počítači (VS Code + Jupyter):
  1) Nainstaluj Python 3.10+ a VS Code.
  2) Ve VS Code nainstaluj rozšíření „Python“ a „Jupyter“ (od Microsoftu).
  3) Vytvoř a aktivuj virtuální prostředí (venv) a nainstaluj balíčky (viz níže).
  4) Otevři sešit `.ipynb` a spusť buňky (Shift+Enter).

## Požadavky a doporučení

- Python 3.10 nebo novější
- Jupyter Notebook/Lab nebo Google Colab
- VS Code (doporučeno) s rozšířeními:
  - Python: <https://marketplace.visualstudio.com/items?itemName=ms-python.python>
  - Jupyter: <https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter>

- Minimální knihovny (ne všechny se používají v každé hodině):
  - NumPy, Pandas, Matplotlib, Seaborn
  - scikit-learn, TensorFlow, PyTorch
  - NetworkX, ipywidgets, Plotly
  - Gradio, transformers (Hugging Face)
  - Pygame (projekty s bludištěm/hry), OR-Tools, python-constraint
  - Ollama (pro lokální LLM experimenty – volitelně)

Poznámka: V Colabu není potřeba nic instalovat předem (většina knihoven je dostupná nebo jde doinstalovat příkazem `pip`).

## Instalace (lokální prostředí)

- Vytvoření a aktivace virtuálního prostředí (macOS/Linux, zsh):

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
# minimální sada – uprav podle potřeby konkrétního sešitu
pip install numpy pandas matplotlib seaborn scikit-learn
# časté doplňky
pip install jupyterlab ipywidgets plotly networkx
# dle lekcí
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
pip install tensorflow
pip install gradio transformers
pip install pygame ortools python-constraint
```

- Spuštění Jupyteru lokálně:

```bash
jupyter lab
# nebo
jupyter notebook
```

- Alternativa: použij Google Colab a soubor nahraj/otevři přímo v prohlížeči: <https://colab.research.google.com>

## Struktura repozitáře

- `AI_Zaklady_Hodina_XX.ipynb` – sešity pro jednotlivé hodiny (případně rozsahy hodin, např. `AI_Zaklady_Hodina_16-17.ipynb`).
- `hourList.md` – kompletní sylabus všech ~60 hodin (téma po tématu).
- `CLAUDE.md` – poznámky ke struktuře projektu a vodítka pro práci s obsahem.
- `source.txt` – seznam vybraných oficiálních dokumentací a zdrojů.
- `WorkResults/` – odevzdané práce studentů (vlastní podsložky).  
  Příklad: `WorkResults/CervenyPetr/` nebo `WorkResults/BigasMartin/`.

Pozor na diakritiku a mezery v názvech složek – doporučeno používat ASCII bez diakritiky a bez mezer:

- ANO: `CervenyPetr`, `Novak_Jan`
- NE: `ČervenýPetr`, `Burger Rico`

## Jak pracovat se sešity

- Každý sešit obsahuje:
  - teoretické vysvětlení (Markdown buňky),
  - praktické Python ukázky,
  - cvičení a úkoly pro studenty,
  - u některých lekcí i mini-projekty (např. bludiště, hry, klasifikace).

- Sešity lze spouštět postupně po buňkách. Pokud nějaký import selže, doinstaluj balíček (viz Instalace) nebo použij Colab.

- Rychlé vyhledání vhodného sešitu:
  - podle názvu `AI_Zaklady_Hodina_XX.ipynb` (číslo hodiny),
  - nebo seřazené v rámci tohoto repozitáře dle názvu.

- Pro přehled témat a návazností použij `hourList.md`.

## Odevzdávání prací (WorkResults)

- Vytvoř si vlastní podsložku: `WorkResults/JmenoPrijmeni/` (bez diakritiky, bez mezer).  
  Příklad: `WorkResults/CervenyPetr`.

- Do své složky umisťuj:
  - vypracované sešity (`.ipynb`) nebo `.py` skripty,
  - soubory s daty (pokud jsou malé),
  - stručný `README.md`/`Navod.txt` s popisem, jak projekt spustit.

- Větší datové soubory nahrávej do cloudu a přidej odkaz (Google Drive, Kaggle Datasets, apod.).

Doporučené minimum v `Navod.txt`/`README.md` u projektu:

- účel/problém, který řešíš,
- seznam knihoven a verze (pokud jsou kritické),
- postup „jak spustit“ (lokálně/Colab),
- ukázkový výstup/snímek obrazovky.

## Přehled sylabu (zkráceně)

Pro kompletní rozpis témat viz `hourList.md`. Vysoká úroveň témat:

- Hodiny 1–10: Úvod do AI, historie, budoucnost, etika, AI kolem nás, hry, mini projekt.
- Hodiny 11–20: Prostor stavů, BFS/DFS, heuristiky a A*, bludiště, projekt.
- Hodiny 21–30: Pravděpodobnost, Bayes, Naivní Bayes, klasifikace v praxi.
- Hodiny 31–40: Strojové učení – zpracování dat, regrese, KNN, vlastní model, vizualizace.
- Hodiny 41–54: Neuronové sítě – perceptron, architektura, aktivace, backprop, dropout, konvoluce, Teachable Machine, projekt.
- Hodiny 55–60: Rizika AI, trh práce, etika a odpovědnost, budoucnost AI, závěr.

## Lokální LLM (Ollama) – volitelně

Některé sešity zmiňují experimenty s LLM přes Ollama. Na macOS lze Ollamu nainstalovat podle oficiální dokumentace: <https://ollama.com/docs>  
Modely jsou pak dostupné lokálně (bez nutnosti cloudu). Instalace modelů a práce s nimi je popsána v dokumentaci Ollamy.

## Nejčastější potíže a řešení (FAQ)

- ImportError / ModuleNotFoundError:  
  Aktivuj virtuální prostředí a nainstaluj chybějící balíček (`pip install ...`). V Colabu přidej buňku s `!pip install ...` a znovu spusť importy.

- Kernel neodpovídá nebo padá:  
  Restartuj kernel (VS Code/Colab), případně zavři a znovu otevři sešit. Zkontroluj paměťové nároky a velikosti datasetů.

- Konflikt verzí knihoven:  
  Použij čisté virtuální prostředí, nebo v Colabu připni verze (`package==x.y.z`).

- Nezobrazují se interaktivní grafy/widgety:  
  Zajisti instalaci a povolení `ipywidgets` a případně použij JupyterLab 3+.

## Jak přidávat/aktualizovat obsah (pro vyučující)

- Nová hodina: zkopíruj existující sešit jako šablonu a přejmenuj na `AI_Zaklady_Hodina_XX.ipynb`.

- U vícedílných lekcí používej formát `AI_Zaklady_Hodina_XX-YY.ipynb`.

- Při přidání nových témat aktualizuj `hourList.md` (navazující struktura, odkazy, poznámky k knihovnám).

- Doplň/aktualizuj odkazy v `source.txt`, pokud přidáš nové knihovny nebo nástroje.

## Oficiální dokumentace a zdroje

Jupyter a Colab:

- Jupyter: <https://docs.jupyter.org/en/latest/>
- Google Colab: <https://colab.research.google.com>

Python a správa prostředí:

- Python venv: <https://docs.python.org/3/library/venv.html>
- pip: <https://pip.pypa.io/en/stable/>
- Conda (alternativa): <https://docs.conda.io/projects/conda/en/stable/>

Datové a vizualizační knihovny:

- NumPy: <https://numpy.org/doc/stable/>
- Pandas: <https://pandas.pydata.org/docs/>
- Matplotlib: <https://matplotlib.org/stable/>
- Seaborn: <https://seaborn.pydata.org/>
- Plotly: <https://plotly.com/python/>
- ipywidgets: <https://ipywidgets.readthedocs.io/en/latest/>

Strojové učení a NN:

- scikit-learn: <https://scikit-learn.org/stable/>
- TensorFlow (guide): <https://www.tensorflow.org/guide>
- PyTorch: <https://pytorch.org/docs/stable/>
- Transformers (Hugging Face): <https://huggingface.co/docs/transformers>

Grafy, hry, optimalizace:

- NetworkX: <https://networkx.org/documentation/stable/>
- Pygame: <https://www.pygame.org/docs/>
- OR-Tools: <https://developers.google.com/optimization>
- python-constraint: <https://pypi.org/project/python-constraint/>

LLM a UI:

- Gradio: <https://www.gradio.app/docs>
- Ollama: <https://ollama.com/docs>

VS Code:

- Python extension: <https://marketplace.visualstudio.com/items?itemName=ms-python.python>
- Jupyter extension: <https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter>

## Licence

Licenční ujednání není v repozitáři uvedeno. Pokud chcete materiály publikovat mimo výuku nebo přidat licenci (např. CC BY-NC-SA), domluvte se prosím v rámci týmu a doplňte `LICENSE`.

## Autoři a kontakt

- Primárně určeno pro výuku předmětu 4IT_GRS1 (2025/26).
- Pro návrhy vylepšení otevři Issue nebo PR, případně kontaktuj správce repozitáře.

---

Užij si učení s AI – a pokud něco nefunguje, začni u „FAQ“ a oficiálních dokumentací výše.
