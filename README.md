# obs-browser-sources

Utility browser sources for OBS Studio.

## pomodoro.html

Clockwork pomodoro timer with auto scene switcher.

![](images/timer.png)

### Usage

Add a browser source with the following URL:

- https://r7kamura.github.io/obs-browser-sources/pomodoro.html

### Change time interval

The default time interval is for 50 min work + 10 min break, linked to the current time:

- Between 00 and 50 minutes, the remaining work time is displayed
- Between 50 and 00 minutes, the remaining break time is displayed

If you would like to change time interval, add `work` and `break` URL query parameters.

For example:

- https://r7kamura.github.io/obs-browser-sources/pomodoro.html?work=25&break=5
  - 25 min work + 5 min break
- https://r7kamura.github.io/obs-browser-sources/pomodoro.html?work=20&break=10
  - 20 min work + 10 min break

### Auto scene switcher

If you set **ADVANCED** permission ("OBS への高度なアクセス" in Japanese) and there are scenes named `Work` and `Break`,
this browser source will automatically switch between the scenes according to the timer.

![](images/obs.png)
