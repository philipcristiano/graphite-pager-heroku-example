# Graphite Pager Heroku Example

Example for running Graphite-Pager on Heroku

## Background

Graphite-Pager is an easy to use alerting tool for Graphite that will send
Pager Duty alerts if a metric reaches a warning or critical level. Heroku
makes deploying Graphite-Pager very simple.


## Requirements

* A Heroku account
* A PagerDury account

## Installation


1. Fork this: `git://github.com/philipcristiano/graphite-pager-heroku-example.git alerts`
2. Register and deploy the application to Heroku
3. Add the Redis-to-Go Add-on

4. Set Environment variables
```
    GRAPHITE_USER=HTTP-basic username
    GRAPHITE_PASS=HTTP-basic password
    GRAPHITE_URL=HTTPS(hopefully) URL to your Graphite installation
    PAGERDUTY_KEY=Specific PagerDuty application key
```
5. Set up alerts in the `alerts.yml` file
6. Push to Heroku!

## Todo

* Test this
* Switch to using a graphite-pager package (when available)
