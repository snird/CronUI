# Cron UI
CronUI provides a simple easy-to-use form for users to specify recurrent events, translated to cron strings.

CronUI is an adoption of the ![jquery-cron](https://github.com/shawnchin/jquery-cron/) project.

CronUI is completely standalone and has no dependencies.

## Usage
```javascript
// Create the ui by initiating new instance of `CronUI`.
// Pass in the selector for the container element of the form,
// and an options object.
recurrentEventForm = new CronUI('.container', {initial: '* * * * *'});
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