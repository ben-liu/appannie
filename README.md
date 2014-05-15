AppAnnie Scripts
================

This repo contains two scripts:

- The **Python** script uses [AppAnnie's](http://www.appannie.com) API to download comments and sales data for every app of each of your accounts.
- The **R** script uses the CSV data generated by the Python script to plot the daily number of downloads of the last 3 years, both per-day and on a 7-day running average.

Simply open `settings.py` and add your API key, then run the script:

```bash
$ ./appannie.py
```

Output
------

The Python script will write several CSV files:

- **Reviews {account}.csv** contains all reviews for all apps of the respective account.
- **Numbers {app-name}.csv** contains daily number of downloads, updates and refunds, plus revenue and refund amounts in your account's currency (I think).

These are simple scripts, if you have accounts with the same name or apps with the same name, one will overwrite the files of another.