nodemates
====

Overview

## Description
This is the tool to use Adventure Mates on the web. Using Node.js, it provides the web-platform of Adventure Mates, which is a traffic simulator.

## Demo


## VS. 

## Requirement
It requires Adventure Mates(http://adventure.sys.t.u-tokyo.ac.jp/download/Mates.html) and you have to compile it before you use it.

## Usage
node start bin/www
Other options can be set w/ config.js

## Install
(You need node & npm & mysql)
1. setting config.js
2. npm install
3. make database
    ```bash:
    sudo mysql
    create database nodemates;
    use nodemates;
    create table `map` (
    `username` varchar(20) default null,
    `mapname` varchar(20) default null,
    `last_update` varchar(20) default null
    );
    create table `user` (
    `username` varchar(20) not null default '',
    `password` varchar(16) default null,
    primary key (`username`)
    );
    CREATE USER 'username' IDENTIFIED BY 'password';
    GRANT ALL on * to 'username';
    ```


## Contribution
1. Fork it
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request

## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)

## Author

[Masanori Hirano](https://github.com/masanorihirano)