# suspend_script

You can suspend your monitoring machine for example, so that it will not run
the whole night.

## Usage
You can create a root cron job that calls this script to execute at a specific time in the evening and then awake in the morning:
```shell
sudo crontab -e
```
Now enter something like to run the suspend script at 23:30:

```shell
30 23 * * * /home/myhomefolder/suspend_until 07:30
```


Used the script from here:
https://askubuntu.com/questions/61708/automatically-sleep-and-wake-up-at-specific-times
