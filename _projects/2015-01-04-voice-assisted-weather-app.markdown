---
layout: project
title:  "VOICE ASSISTED WEATHER APP"
date:   2017-01-04 11:54:46
categories:
- project
img: vawa_thumb.gif
thumb: thumb02.jpg
carousel:
- vawa_01.png
- vawa_02.png
website: https://github.com/kapil93/Voice-Assisted-Weather-App
---
## Voice Assisted Weather App
### Overview
This is a simple weather application which extracts location information from voice commands and displays weather details.

The voice command may or may not have location information but must essentially have a weather intent. In case of absence of location information device location is used.
<br>

![Animation](/assets/img/project/vawa.gif)

<br>

### Project Details
+ This project is built using MVP architecture
+ For speech recognition Android's built-in SpeechRecognizer API is used
+ Retrieval of weather intent and location information from the text obtained from speech recognizer is done by wit.ai service
+ Weather information is obtained using openweathermap.org

<br>
### Libraries Used:
+ Dagger2
+ RxJava