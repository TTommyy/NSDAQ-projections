# Raport z Projektu

## Opis Projektu
Celem projektu było stworzenie modelu prognozujecego cene indeksu giełdowego NASDAQ.
Projekt obejmował przygotowanie danych, budowę i trenowanie modelu, a także jego ewaluację.
Model został zaimplementowany z wykorzystaniem frameworka TensorFlow i biblioteki Keras.

## Dane
Dane odnośnie indexu zostały pobrane ze storny Yahoo Finance, natomiast dane o inflacji ze strony Kaggle.
Zbiór treningowy obejmował lata 1973-2019. Zbiór testowy lata 2020-2023.

## Użyte Metody
1. **Przygotowanie Danych**: Dane zostały wstępnie przetworzone, znormalizowane i podzielone na zestawy treningowe oraz testowe.
2. **Budowa Modelu**: Stworzono sieć neuronową składającą się z kilku warstw LSTM, oraz dropoutów.
3. **Dobór Hiperparametrów**: Najlepsze hiperparametry zostały wybrane za pomocą biblioteki keras_tuner.
4. **Ewaluacja Modelu**: Model został oceniony na zbiorze testowym w celu sprawdzenia jego R2 i innych metryk.

## Uzyskane Rezultaty
Model osiągnął następujące wyniki na zbiorze testowym:
- **R2**: Osiągnięto wynik modelu na poziomie około 0.90.


## Potrzebne Pakiety
Do realizacji projektu niezbędne były następujące pakiety:
- `numpy`
- `pandas`
- `matplotlib`
- `tensorflow`
- `keras`
- `sklearn`
- `keras-tuner`
- `pydot`


Poniżej znajduje się kod instalacji wymaganych pakietów:

```bash
pip install numpy pandas matplotlib tensorflow keras scikit-learn keras-tuner pydot
