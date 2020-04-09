# Installation

We will try to make Installation as easy as possible.

## Requirements

Since LCRM is based on Laravel, all laravel requirements apply

* PHP &gt;= 7.0.0
* OpenSSL PHP Extension
* PDO PHP Extension
* Mbstring PHP Extension
* Tokenizer PHP Extension
* XML PHP Extension

Beside these, you need to have composer installed and since many shared hosting providers doesn't offer ssh, **you may need to use vps**.

### Fresh Installation

This zip file contains all laravel files integrated with Lcrm, however you need to perform following steps to get vendors etc.

### Get Composer packages

Run below command to get all composer packages

```text
composer install
```

### Creating Environment File

Run below commands :

`cp .env.example .env` \(use cp or copy\)

open .env file and modify database details with yours.

### Key Generation

Run below command to get key :

`php artisan key:generate` \(if you use "cp" for copy then use key:gen\)

### compile assets

> If you don't have good knowledge on nodejs and npm, you can copy public folder files from codecanyon's downloaded files

Make sure you have [nodejs](https://nodejs.org) installed in your system with minimum version `6.10.0`,

you can check installed version by running `node -v` command in terminal.

If you are having older version, please install latest version from [nodejs.org](http://nodejs.org/)

For laravel 5.5 , the minimum version of php required is `7.0.0` and

from 5.5 onwards, Laravel team decided to move to webpack from gulp

so assets compilation differs a bit.

They introduced a new npm package for webpack called `mix`

you can read more about it [here](https://laravel.com/docs/5.4/mix).

**install local packages**

`yarn install`

**move assets to public**

`npm run dev`

 **Note:** If bower gives warning that you are running as administrator, please run the command `bower install --allow-root`

## Installation

Before proceeding with the installation process make sure you have your database details ready

Please open your website \(URL/public\) which redirects you to `install` page

follow step by step and finish installation

