# DevOps_CNN
Данный репозиторий содержит сверточную нейронную сеть, построенную на фреймворке Tensorflow с помощью надстройки Keras.
Нейросеть распознает дорожные знаки ограничения скорости 20, 30 и 50 километров.

# Архитектура сети
  * Слой свертки, размер ядра 3х3, количество карт признаков - 32 шт., функция активации ReLU.
  * Слой подвыборки, выбор максимального значения из квадрата 2х2
  * Слой свертки, размер ядра 3х3, количество карт признаков - 32 шт., функция активации ReLU.
  * Слой подвыборки, выбор максимального значения из квадрата 2х2
  * Слой свертки, размер ядра 3х3, количество карт признаков - 64 шт., функция активации ReLU.
  * Слой подвыборки, выбор максимального значения из квадрата 2х2
  * Слой преобразования из двумерного в одномерное представление
  * Полносвязный слой, 64 нейрона, функция активации ReLU.
  * Слой Dropout.
  * Выходной слой, 3 нейрона, функция активации ReLU

# Результаты после обучения
![Results](https://user-images.githubusercontent.com/86290623/174481217-b83f0f68-5f64-4a76-809e-6c95e6b4d22d.png)
