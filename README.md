Yii 2 Advanced Application Template
===================================

Yii 2 Advanced Application Template is a skeleton Yii 2 application best for
developing complex Web applications with multiple tiers.

The template includes three tiers: front end, back end, and console, each of which
is a separate Yii application.

The template is designed to work in a team development environment. It supports
deploying the application in different environments.


DIRECTORY STRUCTURE
-------------------

```
common
    config/              contains shared configurations
    mail/                contains view files for e-mails
    models/              contains model classes used in both backend and frontend
console
    config/              contains console configurations
    controllers/         contains console controllers (commands)
    migrations/          contains database migrations
    models/              contains console-specific model classes
    runtime/             contains files generated during runtime
backend
    assets/              contains application assets such as JavaScript and CSS
    config/              contains backend configurations
    controllers/         contains Web controller classes
    models/              contains backend-specific model classes
    runtime/             contains files generated during runtime
    views/               contains view files for the Web application
    web/                 contains the entry script and Web resources
api
    assets/              contains application assets such as JavaScript and CSS
    config/              contains backend configurations
    controllers/         contains Web controller classes
    models/              contains backend-specific model classes
    runtime/             contains files generated during runtime
    views/               contains view files for the Web application
    web/                 contains the entry script and Web resources
frontend
    node_modules         contains dependent 3rd-party node modules
    bower_components     contains dependent 3rd-party bower components
    test                 contains test files
    app                  contains frontend application
node
    node_modules         contains dependent 3rd-party node modules
vendor/                  contains dependent 3rd-party packages
environments/            contains environment-based overrides
tests                    contains various tests for the advanced application
    codeception/         contains tests developed with Codeception PHP Testing Framework
```


REQUIREMENTS
------------

The minimum requirement by this application template that your Web server supports PHP 5.4.0.


INSTALLATION
------------

If you do not have [Composer](http://getcomposer.org/), you may install it by following the instructions
at [getcomposer.org](http://getcomposer.org/doc/00-intro.md#installation-nix).

If you do not have [NodeJS](https://nodejs.org/), you may install it by following the instructions
at [wiki](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager).

If you do not have [npm](https://npmjs.com/), you may install it by following the instructions
at [docs.npmjs.com](https://docs.npmjs.com/getting-started/installing-node).

If you do not have [bower](http://bower.io/), you may install it by following the instructions
at [bower.io](http://bower.io/#install-bower).

GETTING STARTED
---------------

After you install the application, you have to conduct the following steps to initialize
the installed application. You only need to do these once for all.

1. Run command `init` to initialize the application with a specific environment.
2. Install elasticsearch 1.4.4 on server
3. Composer update
4. Run command from `/path/to/yii-application/frontend/` path `npm install` `bower install`
5. Run command from `/path/to/yii-application/node/` path `npm install`
6. Run command from  `/path/to/yii-application/frontend/` path `grunt serve`
7. Run command from  `/path/to/yii-application/api/` path `php -S localhost:8092`
8. Set document roots of your Web server:

- for frontend `/path/to/yii-application/frontend/` and using the URL `http://localhost:8081/`
- for backend `/path/to/yii-application/node/` and using the URL `http://localhost:8080/`
- for api `/path/to/yii-application/api/web/` and using the URL `http://localhost:8092/`
