# Klasyfikacja obrazów rentgenowskich płuc z wykorzystaniem SOM i SVM

Ten projekt demonstruje klasyfikację obrazów rentgenowskich płuc w celu wykrywania zapalenia płuc przy użyciu Self-Organizing Map (SOM) i Support Vector Machine (SVM).

## Zbiór danych

Zbiór danych użyty w tym projekcie to publiczny zbiór danych obrazów rentgenowskich płuc dostępny na Kaggle. Składa się z zdjęć rentgenowskich klatki piersiowej podzielonych na dwie kategorie: normalne i zapalenie płuc.

## Metoda

Proces klasyfikacji obejmuje następujące kroki:

1. **Załadowanie danych:** Obrazy rentgenowskie są ładowane ze zbioru danych i dzielone na zbiory treningowe, walidacyjne i testowe.
2. **Przetwarzanie wstępne:** Obrazy są przetwarzane wstępnie przy użyciu ImageDataGenerator w celu rozszerzenia zbioru danych i ekstrakcji cech przy użyciu VGG16.
3. **Trening SOM:** SOM jest szkolona na preprocesowanych danych w celu redukcji wymiarowości i grupowania podobnych obrazów.
4. **Trening SVM:** SVM jest szkolony na danych zredukowanych przy użyciu SOM w celu klasyfikacji obrazów jako normalnych lub zapalenia płuc.
5. **Ewaluacja:** Wydajność modelu jest oceniana na zbiorze testowym przy użyciu różnych metryk, takich jak dokładność, precyzja i czułość.

## Wyniki

Model osiągnął wysoką dokładność w klasyfikacji obrazów rentgenowskich płuc, demonstrując potencjał SOM i SVM w diagnostyce medycznej.

## Wymagania

Do uruchomienia tego projektu wymagane są następujące biblioteki:

* TensorFlow
* Keras
* MiniSom
* Scikit-learn
* Matplotlib
* Seaborn

## Użycie

1. Sklonuj repozytorium.
2. Pobierz zbiór danych i umieść go w katalogu `data`.
3. Uruchom notebook Jupyter `pneumonia_classification.ipynb`.

## Uwagi

* Ten projekt ma na celu demonstrację i może wymagać dalszych ulepszeń w przypadku zastosowań w świecie rzeczywistym.
* Zbiór danych użyty w tym projekcie jest stosunkowo niewielki i może nie odzwierciedlać złożoności rzeczywistych scenariuszy klinicznych.
