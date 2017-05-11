# SCCounter
Simple responsive **HTML5/JavaScript** D-day counter.<br><br>
## Demo Screenshot(desktop)
![DEMO IMG](https://github.com/SoyaNyan/SCCounter/blob/master/demo.PNG)
## Releases now available
**Pre-release version** is now availalbe at [**release page**](https://github.com/SoyaNyan/SCCounter/releases). <br>
Feek free to give us **feedback** or **comment** below if you have any good idea.
## How to install
1. Simply download the project and upload to your hosting directory.
2. Set counter's start & end time using epoch time convertor(see below).
3. Customize style editing code **"style.css"** or **"jquery.final-countdown.js"**(optional).
4. That's it!
## Easly customizable
* Counter style(borderColor, borderWidth, position... etc.)
* Counter times
* Change favicon(.ico) or background img(.jpg .png)
* More functions can be added if you need.
### Counter time setting guide(index.php)
Fix time value just like the code below...
```html
<script type="text/javascript">
  $('.countdown').final_countdown({
    start: '[start time here(epoch)]',
    end: '[end time here(epoch)]',
    now: 'new Date().getTime() / 1000' // fixed; automatically get current time from system
  });
</script>
```
### Counter style option setting guide(js/jquery.final-countdown.js)
Fix **borderColor(hex)** and **borderWidth** value...
```javascript
// Timer borderColor, borderWidth settings
    var defaults = $.extend({
        start: undefined,
        end: undefined,
        now: undefined,
        selectors: {
            value_seconds: '.clock-seconds .val',
            canvas_seconds: 'canvas-seconds',
            value_minutes: '.clock-minutes .val',
            canvas_minutes: 'canvas-minutes',
            value_hours: '.clock-hours .val',
            canvas_hours: 'canvas-hours',
            value_days: '.clock-days .val',
            canvas_days: 'canvas-days'
        },
        seconds: {
            borderColor: '#7995D5', // color setting
            borderWidth: '6' // border weight setting
        },
        minutes: {
            borderColor: '#ACC742', // color setting
            borderWidth: '6' // border weight setting
        },
        hours: {
            borderColor: '#ECEFCB', // color setting
            borderWidth: '6' // border weight setting
        },
        days: {
            borderColor: '#FF9900', // color setting
            borderWidth: '6' // border weight setting
        }
    }, options);
```
### Change favicon and background image
1. Goto *"img"* directory.
2. Just upload your new **"favicon.ico"** and **"background.jpg"** file.
```css
html {
  background-image: url('background.jpg'); // background img file route
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
}
```
In case if you want to use .png file, fix **"style.css"**
#### Epoch time convertor
* <https://www.epochconverter.com/>
* <http://www.unixtimestamp.com/index.php>
###### Original Plugin
This awesome jQuery plugin is developed by **PragmaticMates**. <br>
For more Advanced Usages, please check the **demo page** or visit the [**official website**](http://www.jqueryscript.net/time-clock/Modern-Circular-jQuery-Countdown-Timer-Plugin-Final-Countdown.html).
