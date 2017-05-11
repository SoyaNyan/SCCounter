# SCCounter
Simple responsive HTML5/JavaScript D-day counter.<br><br>
## Demo Screenshot(desktop)
![DEMO IMG](https://github.com/SoyaNyan/SCCounter/blob/master/demo.PNG)
## How to install
1. Simply download the project and upload to your hosting directory.
2. Set counter's start & end time using epoch time convertor(see below).
3. Customize style editing code *"style.css"* or *"jquery.final-countdown.js"*(optional).
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
#### Epoch time convertor
* <https://www.epochconverter.com/>
* <http://www.unixtimestamp.com/index.php>
###### Original Plugin
This awesome jQuery plugin is developed by PragmaticMates. 
For more Advanced Usages, please check the demo page or visit the [official website](http://www.jqueryscript.net/time-clock/Modern-Circular-jQuery-Countdown-Timer-Plugin-Final-Countdown.html).
