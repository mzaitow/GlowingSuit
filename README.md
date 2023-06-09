# Танцевальный костюм с подсветкой
## Нога костюма
### 1. Какие компоненты используются? 
  Для данной части костюма была использована аппаратная платформа Arduino, \
  которая считывает показания с модуля, содержащего в себе гироскоп и акселерометр, \
  и управляет двумя светодиодными лентами исходя из полученных ей данных. Все компоненты \
  питаются от аккумулятора, который контролируется специальным контроллером.
### 2. Какие модели компонентов использованы?
1. Аппаратная платформа Arduino Nano. Имеет достаточно малый уровень энергопотребления \
  и небольшие габариты.
3. Модуль GY-521, содержащий в себе акселерометр и гироскоп.
4. Светодиодная лента WS2812B. RGB-лента, с помощью которой можно реализовать различные \
  световые эффекты.
6. Светодиодный модуль питания HW-107. Позволяет сделать данный модуль всего костюма \
  автономным за счёт использования литий-ионного аккумулятора (*или павербанка, что использовано в \
  прототипе*), контролем заряда которой и занимается данный модуль.
5. Литий-ионная батарея.
### 3. Как работает?
  Arduino считывает показания с гироскопического датчика по одной из осей. Датчик заранее откалиброван \
  для того, чтобы его можно было закрепить на верхней части стопы посередине. \
  Исходя из полученных с датчика данных на светодиодные ленты передаётся идентичный сигнал с \
  определённым эффектом (*в случае с данным прототипом это простые изменяющиеся столбики света*).
#### Схема
  ![](https://raw.githubusercontent.com/mzaitow/GlowingSuit/main/leg_scheme.png)
  
#### Прототип
  ![](https://github.com/mzaitow/GlowingSuit/blob/main/2023-06-1512:57:27124x426.png?raw=true)
