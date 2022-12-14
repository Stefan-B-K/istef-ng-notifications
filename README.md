# IstefNgNotifications

Basic notifications widget for your Angular projects.  
Clips to the bottom right of the web page.  
Message type/color :   success / green  -  error / red  -  info / blue  

![](https://github.com/Stefan-B-K/istef-ng-notifications/blob/main/src/assets/Screenshot.png)

## Install

`
npm i istef-ng-notifications
`

## Use

Add `<istef-ng-notifications></istef-ng-notifications>` to the component html, where you want notifications displayed.

Inject <b><i>`NotificationsService`</i></b>  in your service/s and call the corresponding method:
* <i>`addSuccessMessage()`</i>
* <i>`addErrorMessage()`</i>
* <i>`addInfoMessage()`</i>

like that: 
```
.pipe(
    tap(  
        () => this.notifications.addSuccessMessage('...'),
        (err) => this.notifications.addErrorMessage('...', 10)
)
```
where the second argument (<i>optional</i>) is the display time of the notification (<i>in seconds, default 5s</i>).

## Other

This library was generated with [Angular CLI](https://github.com/angular/angular-cli) version 14.0.0.
