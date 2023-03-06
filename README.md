# Usage of Composer and PHPMetrics via Docker

Installation of PHPMetrics package   

```docker run --rm --interactive --tty --volume $PWD:/app composer require-dev phpmetrics/phpmetrics```

Creating a report for the directory **./src** 

```docker run --rm --interactive --tty --volume $PWD:/app composer php ./vendor/bin/phpmetrics --report-html=THE_REPORT_DIRECTORY ./src```