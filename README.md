(
just a repackaging so that it will work with npm

```
npm install cron-ui
CronUI = require 'cron-ui'
```
)

# Cron UI
CronUI provides a simple easy-to-use form for users to specify recurrent events, translated to cron strings.

CronUI is an adaption of the [jquery-cron](https://github.com/shawnchin/jquery-cron/) project.

CronUI is completely standalone and has no dependencies.

Visit the [CronUI page](https://snird.github.io/CronUI/) for docs and examples.

## Usage
```javascript
// Create the ui by initiating new instance of `CronUI`.
// Pass in an element selector or DOM element by itself to render
// the form in, and options object.
recurrentEventForm = new CronUI('.container', {initial: '* * * * *'});
// With DOM element
var el = document.querySelector('.my-container');
new CronUI(el, {initial: '0 5 * * *'});
```

## Functionality
Currently CronUI only supports a subset of cron abilities.
- Only support digits
- No commas for multiple entries

These are the possible combinations so far:
- Every minute : * * * * *
- Every hour   : ? * * * *
- Every day    : ? ? * * *
- Every week   : ? ? * * ?
- Every month  : ? ? ? * *
- Every year   : ? ? ? ? *
