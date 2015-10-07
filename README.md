# Introduction

[AngularJS 2](https://angular.io/) implementation of the [RDash admin dashboard](http://rdash.github.io) theme

**Note:** Angular 2.0 is not production ready yet! This seed project is perfect for playing around with the latest versions but do not start new projects with it since a lot of new changes are going to be introduced until the framework is officially released.


[**Demo App**](https://rdash-angular2.herokuapp.com/)

_*Based on [angular2-seed](https://github.com/mgechev/angular2-seed) project*_

# How to start

```bash
git clone https://github.com/ziyasal/rdash-angular2.git
cd rdash-angular2
npm install
# dev
npm run serve.dev
```
_Does not rely on any global dependencies._

# Configuration

Default application server configuration

```javascript
var PORT             = 5555;
var LIVE_RELOAD_PORT = 4002;
var APP_BASE         = '/';
```

Configure at runtime

```bash
npm run serve.dev -- --port 8080 --reload-port 4000 --base /my-app/
```

## Directives

- RdWidget
- RdWidgetHeader
- RdWidgetBody
- RdWidgetFooter
- RdLoading


**Simple Widget** 
```js
    <rd-widget>
      <rd-widget-body>       
       <span>HTML CONTENT</span>       
      </rd-widget-body>
    </rd-widget>
```

**Widget with Header**  
```js
 <rd-widget>
       <rd-widget-header icon="fa-tasks" title="Servers">
         <a href="javascript:void(0)" style="float: right">Manage</a>
       </rd-widget-header>
       <rd-widget-body classes="medium no-padding">
         <server-list-view [model]="servers"></server-list-view>
       </rd-widget-body>
     </rd-widget>
```

**Widget with Footer**  
```js
 <rd-widget>
       <rd-widget-header icon="fa-tasks" title="Servers">
         <a href="javascript:void(0)" style="float: right">Manage</a>
       </rd-widget-header>
       <rd-widget-body classes="medium no-padding">
         <server-list-view [model]="servers"></server-list-view>
       </rd-widget-body>
       <rd-widget-footer>
         <span>FOOTER CONTENT</span>
       </rd-widget-footer>
     </rd-widget>
```

**Widget with Loader**  
```js
 <rd-widget>
    <rd-widget-body classes="medium no-padding">
       <rd-loading></rd-loading>
    </rd-widget-body>
 </rd-widget>
```

# Change Log

You can follow the [Angular 2 change log here](https://github.com/angular/angular/blob/master/CHANGELOG.md).

# License

[MIT](https://raw.githubusercontent.com/ziyasal/rdash-angular2/master/LICENSE)