Titanic EDA — Who Survived, and Why?
A short, reproducible exploratory data analysis (no modeling) of the classic Titanic passenger dataset, built to be read end-to-end in about two minutes.

What's here
notebooks/titanic_eda.ipynb — the notebook. Loads the data, cleans it with documented reasoning for each decision, and closes with a ~150-word findings section plus next steps.
data/titanic.csv — the raw dataset (891 passengers), included in the repo so the notebook runs offline with no download step.
requirements.txt — pinned versions of pandas, numpy, matplotlib, seaborn, and jupyter.
How to run it
git clone <this-repo-url>
cd titanic-eda
python3 -m venv .venv && source .venv/bin/activate   # optional but recommended
pip install -r requirements.txt
jupyter notebook notebooks/titanic_eda.ipynb
Then Kernel → Restart & Run All. The notebook only depends on the relative path ../data/titanic.csv, so it works the same on any machine that clones the repo — no hardcoded local paths.

What I did
Loaded the raw CSV in a single cell.
Audited missingness (Age, Cabin, Embarked) before touching anything.
Cleaned each column with a documented reason: median-imputed Age (skewed distribution), mode-imputed the 2 missing Embarked values, and turned the 77%-missing Cabin column into a HasCabin flag rather than inventing values. Engineered FamilySize, IsAlone, and AgeGroup for the analysis.
Explored survival by sex, class, their interaction, age group, and family size, using a small number of charts chosen to build one narrative rather than a chart dump.
Summarized the "who survived and why" story and what I'd investigate next with more time (title extraction, fare/ticket-sharing, a baseline model).
Key finding (see notebook for full writeup)
Survival was driven mainly by sex and class, and the two compounded each other — first-class women survived at ~97% versus ~14% for third-class men. Age mattered at the margins, consistent with a "women and children first" evacuation pattern.

Tech used
Python, pandas, NumPy, matplotlib, seaborn, Jupyter.
