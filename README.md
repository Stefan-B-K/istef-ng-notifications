# IstefNgNotifications

Basic notifications list/widget for your Angular projects. 
Clips the list of messages to the bottom right of the web page.
Message type/color :   success / green  -  error / red  -  info / blue

## Install

`
npm i istef-ng-notifications
`

## Use

Add `<istef-ng-notifications></istef-ng-notifications>` to the component html, where you want notifications displayed.

Inject <span style="color: green">NotificationListComponent</span>  in your service/s and call the corresponding method:
* <span style="color: #13cc70">addSuccessMessage()</span>
* <span style="color: #13cc70">addErrorMessage()</span>
* <span style="color: #13cc70">addInfoMessage()</span>

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
