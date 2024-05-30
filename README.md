# Klasyfikacja-tytu-w-szachowych
Projekt skupia się na budowie optymalnego modelu uczenia maszynowego do klasyfikacji tytułów szachowych graczy na podstawie ich rankingów w różnych trybach gry (standardowy, rapid i blitz). Zadanie to realizuję w języku programowania R.

## Opis Projektu
Celem tego projektu jest opracowanie solidnego modelu klasyfikacyjnego, który będzie w stanie dokładnie przewidywać tytuły szachowe graczy (np. Arcymistrz, Mistrz Międzynarodowy) na podstawie ich rankingów w różnych trybach gry.

## Przygotowanie Danych
Rozpocząłem od wczytania i przetworzenia danych, usuwając brakujące i niepotrzebne wartości, aby zapewnić ich jakość i spójność. Następnie przeprowadziłem analizę korelacji między zmiennymi, aby zidentyfikować istotne cechy wpływające na klasyfikację tytułów. W tym etapie uzupełniałem również brakujące dane, aby zapewnić kompletność zestawu danych.

## Budowa Modeli
Podzieliłem dane na zestawy treningowe i testowe, a następnie przystąpiłem do budowy różnych modeli uczenia maszynowego:

### Drzewa Decyzyjne:
Korzystając z pakietów rpart i parsnip, zbudowałem modele drzew decyzyjnych, które zostały następnie zweryfikowane i dostrojone za pomocą walidacji krzyżowej. Analizowałem wyniki, tworzyłem macierze pomyłek i dostosowywałem modele poprzez przycinanie drzew decyzyjnych.

### Las Losowy:
Wdrożyłem model lasu losowego, który został zoptymalizowany poprzez strojenie hiperparametrów i walidację krzyżową. Oceniłem dokładność modelu na danych testowych.

### XGBoost: 
Zaimplementowałem model XGBoost, który również przeszedł proces strojenia hiperparametrów i walidacji krzyżowej. Wyniki zostały ocenione za pomocą odpowiednich metryk.

### K-Najbliższych Sąsiadów (kNN):
Przeanalizowałem różne wartości k dla k-nearest neighbors, budując modele i oceniając ich skuteczność w przewidywaniu tytułów szachowych.

### Metoda Wektorów Nośnych (SVM):
Zbudowałem model SVM, który został następnie zweryfikowany na danych testowych. Przeprowadziłem także dodatkowe analizy, takie jak porównanie wyników dla kobiet i mężczyzn.

### Sieci Neuronowe:
Zdefiniowałem i dostroiłem sieć neuronową, korzystając z technik takich jak Grid Search do optymalizacji hiperparametrów. Analizowałem wyniki przy użyciu trójwymiarowych wizualizacji danych.

## Ewaluacja i Wyniki
Każdy model został dokładnie oceniony pod kątem dokładności, precyzji, czułości i innych kluczowych metryk. Porównywałem wyniki, aby zidentyfikować najlepszy model dla klasyfikacji tytułów szachowych.

## Technologie i Biblioteki
Język R: Wykorzystanie R do analizy danych i budowy modeli uczenia maszynowego.
Pakiety R: m.in. rpart, parsnip, randomForest, xgboost, class, e1071, nnet.
Wnioski
Projekt przedstawia kompleksowe podejście do klasyfikacji tytułów szachowych z wykorzystaniem zaawansowanych technik uczenia maszynowego. Każdy etap, od przygotowania danych, przez budowę i walidację modeli, po ostateczną ocenę, jest szczegółowo opisany i zrealizowany w języku R.
