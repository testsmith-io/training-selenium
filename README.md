# Training TestNG Selenium WebDriver Project

![Badge](https://github.com/testsmith-io/training-testng-selenium-webdriver/actions/workflows/maven.yml/badge.svg)


This project is generated from an archetype. It exists out of TestNG, Selenium WebDriver, WebDriver Manager, Allure and
OWNER as the main dependendies.

The following browsers can be used:
`CHROME`, `FIREFOX`, `EDGE`, `OPERA`, `INTERNET_EXPLORER` and `CHROME_HEADLESS`

## Run tests

The following Maven profiles can be used:

### Prestashop

`mvn clean test -P prestashop-exercises`

`mvn clean test -P prestashop-answers`

By default, Chrome will be used. To override the default browser, you can use the following command (and choose one of
the supporting browsers):

`mvn clean test -P prestashop-answers -DseleniumBrowser=firefox`

### Parabank

`mvn clean test -P parabank-exercises`

`mvn clean test -P parabank-answers`

By default, Chrome will be used. To override the default browser, you can use the following command (and choose one of
the supporting browsers):

`mvn clean test -P parabank-answers -DseleniumBrowser=firefox`

### Prestashop (using docker)

`mvn clean test -P prestashop-exercises-docker`

`mvn clean test -P prestashop-answers-docker`

By default, Chrome will be used. To override the default browser, you can use the following command (and choose `firefox`, `chrome` or `edge`):

`mvn clean test -P prestashop-answers-docker -DseleniumBrowser=firefox`

### Parabank (using docker)

`mvn clean test -P parabank-exercises-docker`

`mvn clean test -P parabank-answers-docker`

By default, Chrome will be used. To override the default browser, you can use the following command (and choose `firefox`, `chrome` or `edge`):

`mvn clean test -P parabank-answers-docker -DseleniumBrowser=firefox`

## Generate report

`mvn allure:report`

`mvn allure:serve`

## Display dependency updates

`mvn versions:display-dependency-updates`
