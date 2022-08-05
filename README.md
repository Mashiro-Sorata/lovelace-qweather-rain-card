# Home Assistant QWeather Forecast Card
Graph of QWeather rain forecast 
和风天气-降雨量卡片
修改自[lukevink/lovelace-buien-rain-card](https://github.com/lukevink/lovelace-buien-rain-card)

如果想要免费使用和风天气的API，使用前需要[注册和风天气](https://id.qweather.com/#/register?redirect=https%3A%2F%2Fconsole.qweather.com)的账号并完成实名制，成为[免费开发版开发者(Free Dev Developer)](https://dev.qweather.com/help/general/)。

![Preview Image](https://github.com/Mashiro-Sorata/lovelace-qweather-rain-card/blob/master/qweather-card-screenshot1.png?raw=true)

### Simple install

1. Download and copy `qweather-rain-card.js` into your `config/www` directory.

2. Add a reference to `qweather-rain-card.js` inside your `ui-lovelace.yaml`.

  ```yaml
  resources:
    - url: /local/qweather-rain-card.js
      type: module
  ```

### Add as a card to your UI

      - type: 'custom:qweather-rain-forecast'
        qweather_key: ********************************
        long: 104.06
        lat: 30.67
        lineColor: 'rgba(89, 160, 238, 1)'
        fillColor: 'rgba(89, 160, 238, 0.2)'
        update_interval: 60
        icon: 'mdi:weather-rainy'
        
 (update interval is in seconds)

### An example in my own UI as a Picture Element:

![Preview Image](https://github.com/Mashiro-Sorata/lovelace-qweather-rain-card/blob/master/qweather-card-screenshot2.png?raw=true)
