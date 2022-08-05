# Home Assistant QWeather Forecast Card
Graph of QWeather rain forecast 
和风天气-降雨量卡片
修改自[lukevink/lovelace-buien-rain-card](https://github.com/lukevink/lovelace-buien-rain-card)

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
        long: 104.06
        lat: 30.67
        lineColor: 'rgba(89, 160, 238, 1)'
        fillColor: 'rgba(89, 160, 238, 0.2)'
        update_interval: 60
        icon: 'mdi:weather-rainy'
        
 (update interval is in seconds)

### An example in my own UI as a Picture Element:

![Preview Image](https://github.com/Mashiro-Sorata/lovelace-qweather-rain-card/blob/master/qweather-card-screenshot2.png?raw=true)
