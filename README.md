# What is PingMeLive?

This is a library which helps you to get LIVE notifications of actions taking place on your webistes and applications.
Just Copy past the below codes and get live updates of errors and actions. Make Categories of pings based on projects (etc) and assign it to your team mates.
That's what PING ME LIVE does.
Easy right!.

## How to use

### Register yourself on
[https://pingmelive.com](https://pingmelive.com)
You will get your API KEY after registeration.


### Usage

Include pingmelive
```php
<?php
require_once("pingmelive.lib.php");
$pingmelive = new pingMeLive(apiKey,projectID,errorStatus,errorName); 
?>

```

...and you are done!

## Custom Events

You can also use pingMeLive for sending custom events.

### 1.Simple event
```html
$pingMeLive->simpleEvent(groupTitle,eventMessage);
 ```    

If you want to send some detailed long description you can use `Detailed event`
### 2.Detailed event
```html
$pingMeLive->detailedEvent(groupTitle,eventMessage,detailDescription);
```

### Options
* apiKey : You will get an `API KEY` when you will register on pingmelive.com
* projectID : You will get an `APP ID` when you will register on pingmelive.com 
* errorStatus : true / false
* errorName : 
* groupTitle : 
* eventMessage :
* detailDescription : 

## Some usefull information

* Only `Detailed event` will by default contain the information like device info,app version code etc.
* If you only want error event just install the library and thats it, no need to code anything else.
* You can smartly use group title for you custom events.

