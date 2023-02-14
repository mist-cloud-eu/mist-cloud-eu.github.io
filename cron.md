# Cron jobs in mist-cloud

In order to run code at fixed intervals in mist-cloud we can use _cron jobs_. A mist cron job is a mechanism that can be configured to post custom events to the rapids at fixed times. For example, every 5 minutes (`*/5 * * * *`), or the last weekday of every month (`0 0 L * *`).

Our syntax of cron has 5-6 elements:
* Seconds (optional)
* Minutes
* Hours
* Day of month, where L is last weekday
* Month, where 1 is January
* Day of week, where 1 is Monday

To set up a cron job simply use the command:

```
mist cron [name] --expr "[cron expression]" --event [event to post]
```

> ⚠ Things to note:
> * If event is omitted the name is used. 
> * A cron event is posted without payload, and replies have no effect. 
> * Cron jobs are organization wide.
> * To prevent accidental updates mist-cli requires you to specify `--overwrite` if you want to modify an existing cron job. 

You can delete a cron job by specifying an empty expression (`""`). And finally you can list your current cron jobs with the command:

```
mist list-crons
```
