# Laravel Backup

We used "laravel filesystem" to backup the files and Database. We can save the files into Local and Dropbox. Mention the file names in`config/backup.php`which you want Back Up. You can include and exclude the files here.

Run the below command for Back Up.

```text
php artisan backup:run
```

For clean/clearing the Back Up run the below command

```text
php artisan backup:clean
```

Referral Links:

[https://laravel.com/docs/5.5/filesystem](https://laravel.com/docs/5.5/filesystem)

[https://github.com/spatie/laravel-backup](https://github.com/spatie/laravel-backup)

