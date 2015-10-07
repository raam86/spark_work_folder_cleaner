#SPARK WORKERS WORK FOLDER CLEANER

spark standalone cluster doesn't clear the older works of running application. 
Since spark streaming rarely stops this bash script will clean the work folder from the master to all of your slaves. 


### How to use

1)pull the repo
2)add the cron line with the correct path (paste into crontab -e)
3)profit 

*Cron Line*
32 * * * * /home/ubuntu/distrbute_to_workers  > clean_workers_work_folder.log
