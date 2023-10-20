# machine-learning

Breast Cancer Classification using Perceptron

Opis projektu

Projekt ten wykorzystuje algorytm Perceptron do klasyfikacji guzów nowotworowych jako złośliwych lub łagodnych na podstawie cezji opisujących te guzy. Dane opisują stan guzów nowotworowych, a w kolumnie "diagnosis" zawiera informację o tym, czy guz jest złośliwy (M) czy łagodny (B).

Instrukcje

Importujemy potrzebne biblioteki, takie jak numpy, pandas, StandardScaler z sklearn.preprocessing, train_test_split z sklearn.model_selection, oraz Perceptron z sklearn.linear_model.
Wczytujemy dane z pliku "breast_cancer.csv" za pomocą pandas i zapisujemy je w zmiennej diag.
Przygotowujemy dane:
Wybieramy wybrane kolumny (cechy) z danych, takie jak 'area_mean', 'area_se', 'texture_mean', 'concavity_worst', 'concavity_mean', i zapisujemy je w zmiennej X.
Wybieramy kolumnę 'diagnosis' i przekształcamy wartości "M" na 1 (złośliwe) i pozostałe na -1 (łagodne) w zmiennej y.
Standaryzujemy dane za pomocą StandardScaler, aby mieć średnią równą 0 i odchylenie standardowe równa 1, a wyniki zapisujemy w zmiennej X_std.
Dzielimy dane na zbiór treningowy (80% danych) i zbiór testowy (20% danych) za pomocą train_test_split, a wyniki zapisujemy w zmiennych X_train, X_test, y_train, i y_test.
Tworzymy model Perceptron z określonymi parametrami, takimi jak eta0 (współczynnik uczenia) i max_iter (maksymalna liczba iteracji).
Trenujemy model Perceptron na danych treningowych za pomocą fit.
Przewidujemy wartości na danych testowych i wyniki zapisujemy w zmiennej y_pred.
Obliczamy i wyświetlamy wyniki:
Porównujemy przewidziane wartości y_pred z rzeczywistymi wartościami y_test, aby obliczyć liczbę poprawnie przewidzianych wartości (zmienna good).
Obliczamy procent poprawnych odpowiedzi i wyświetlamy go na ekranie.

Ten projekt ilustruje proces klasyfikacji przy użyciu algorytmu Perceptron i może być wykorzystany do oceny, czy guzy nowotworowe są złośliwe czy łagodne na podstawie podanych cezji.
