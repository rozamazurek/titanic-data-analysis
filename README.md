# Titanic – analiza danych i model klasyfikacyjny

Repozytorium zawiera dwa notebooki Jupyter realizujące pełny proces analizy danych oraz budowy modeli uczenia maszynowego na zbiorze danych Titanic.

---

## Zawartość projektu

Projekt składa się z dwóch głównych części:

1. **titanic-data-basic-statistics.ipynb**  
   - eksploracyjna analiza danych 
   - statystyki opisowe  
   - wizualizacje  
   - analiza braków danych  

2. **titanic-classifying-model.ipynb**  
   - przygotowanie danych do modelowania  
   - budowa pipeline’ów ML  
   - trenowanie i ewaluacja modeli  
   - porównanie wyników

---

## Wykorzystane technologie

Projekt został wykonany w oparciu o:

- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- xgboost  
- Jupyter Notebook 

---

## Wykorzystane modele klasyfikacyjne

W notebooku klasyfikacyjnym przetestowano **5 różnych modeli uczenia maszynowego**:

1. **DummyClassifier** – model bazowy do porównania  
2. **LogisticRegression** – regresja logistyczna  
3. **RandomForestClassifier** – las losowy  
4. **KNeighborsClassifier** – klasyfikator k-najbliższych sąsiadów  
5. **XGBClassifier** – model gradient boosting z biblioteki XGBoost  

Dla każdego modelu przeprowadzono:

- trening na zbiorze treningowym  
- predykcje na zbiorze testowym  
- ocenę jakości (accuracy, inne metryki)  
- porównanie skuteczności między modelami  

---

## Struktura repozytorium

```
├── titanic-data-basic-statistics.ipynb   # analiza i eksploracja danych
├── titanic-classifying-model.ipynb       # budowa i ocena modeli
└── requirements.txt                      # zbiór uytych bibliotek
```

---

## Jak uruchomić projekt

### 1. Pobranie repozytorium

```bash
git clone <adres-repozytorium>
cd <nazwa-folderu>
```

### 2. Pobranie zbioru danych

Projekt korzysta z publicznego zbioru danych Titanic dostępnego na Kaggle:

https://www.kaggle.com/datasets/yasserh/titanic-dataset

Pobierz plik CSV z powyższej strony, a następnie:

- umieść go na swoim koncie **Google Drive**,  
- lub zapisz lokalnie w folderze projektu pod nazwą `titanic.csv`.

Notebooki zostały przygotowane do pracy z plikiem wczytywanym z Google Drive (tak jak w kodzie źródłowym).

### 3. Instalacja wymaganych bibliotek

Wszystkie wymagane zależności znajdują się w pliku `requirements.txt`.

Aby je zainstalować, wystarczy wykonać:

```bash
pip install -r requirements.txt
```

### 4. Uruchomienie notebooków

Projekt można uruchomić na dwa sposoby:

#### Lokalnie:

```bash
jupyter notebook
```

i otworzyć jeden z notebooków:

- `titanic-data-basic-statistics.ipynb`
- `titanic-classifying-model.ipynb`

#### W Google Colab:

- wgraj notebook do Google Colab,  
- zamontuj Google Drive (zgodnie z kodem w notebookach),  
- upewnij się, że plik z danymi Titanic znajduje się na Twoim Google Drive w odpowiedniej lokalizacji.

---

Po wykonaniu powyższych kroków notebooki są gotowe do uruchomienia bez dodatkowej konfiguracji.

## Dane wejściowe

Projekt wykorzystuje klasyczny zbiór danych **Titanic Dataset**, zawierający m.in.:

- wiek pasażera  
- płeć  
- klasę biletu  
- cenę biletu  
- port zaokrętowania  
- informację o przeżyciu  

Dane są przetwarzane, czyszczone i przygotowywane przed przekazaniem do modeli ML.

---

## Możliwe rozszerzenia

Projekt można dalej rozwijać poprzez:

- tuning hiperparametrów  
- feature engineering  
- walidację krzyżową  
- testowanie dodatkowych modeli  

---

## Autor

Projekt wykonany w ramach Wakacyjnego Wyzwania organizowanego przez Koło Naukowe Solvro.

---