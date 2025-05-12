Node.js User Management System - Express, Express-Handlebars, HBS, MySQL

Create .env file
Create a .env file to store your database credentials

DB_HOST = localhost
DB_NAME = usermanagement_tut
DB_USER = root
DB_PASS = password
Installation
To run this project, install it locally using npm:

$ npm install
$ npm start


SQL Workbench ==>


1.  Create database user_management

2.  use user_management;

3.  CREATE TABLE `user` (
    `id` INT NOT NULL AUTO_INCREMENT,
    `first_name` VARCHAR(45) NOT NULL,
    `last_name` VARCHAR(45) NOT NULL,
    `email` VARCHAR(45) NOT NULL,
    `phone` VARCHAR(45) NOT NULL,
    `comments` TEXT NOT NULL,
    `status` VARCHAR(10) NOT NULL DEFAULT 'active',
    PRIMARY KEY (`id`)
    ) ENGINE=InnoDB;


4.  Select * from user;


5.  INSERT INTO `user` 
  (`id`, `first_name`, `last_name`, `email`, `phone`, `comments`, `status`) 
  VALUES
  (NULL, 'Amanda',    'Nunes',         'anunes@ufc.com',        '012345678910', '', 'active'),
  (NULL, 'Alexander', 'Volkanovski',   'avolkanovski@ufc.com',  '012345678910', '', 'active'),
  (NULL, 'Khabib',    'Nurmagomedov',  'knurmagomedov@ufc.com', '012345678910', '', 'active'),
  (NULL, 'Kamaru',    'Usman',         'kusman@ufc.com',        '012345678910', '', 'active'),
  (NULL, 'Israel',    'Adesanya',      'iadesanya@ufc.com',     '012345678910', '', 'active'),
  (NULL, 'Henry',     'Cejudo',        'hcejudo@ufc.com',       '012345678910', '', 'active'),
  (NULL, 'Valentina', 'Shevchenko',    'vshevchenko@ufc.com',   '012345678910', '', 'active'),
  (NULL, 'Tyron',     'Woodley',       'twoodley@ufc.com',      '012345678910', '', 'active'),
  (NULL, 'Rose',      'Namajunas',     'rnamajunas@ufc.com',    '012345678910', '', 'active'),
  (NULL, 'Tony',      'Ferguson',      'tferguson@ufc.com',     '012345678910', '', 'active'),
  (NULL, 'Jorge',     'Masvidal',      'jmasvidal@ufc.com',     '012345678910', '', 'active'),
  (NULL, 'Nate',      'Diaz',          'ndiaz@ufc.com',         '012345678910', '', 'active'),
  (NULL, 'Conor',     'McGregor',      'cmcgregor@ufc.com',     '012345678910', '', 'active'),
  (NULL, 'Cris',      'Cyborg',        'ccyborg@ufc.com',       '012345678910', '', 'active'),
  (NULL, 'Tecia',     'Torres',        'ttorres@ufc.com',       '012345678910', '', 'active'),
  (NULL, 'Ronda',     'Rousey',        'rrousey@ufc.com',       '012345678910', '', 'active'),
  (NULL, 'Holly',     'Holm',          'hholm@ufc.com',         '012345678910', '', 'active'),
  (NULL, 'Joanna',    'Jedrzejczyk',   'jjedrzejczyk@ufc.com',  '012345678910', '', 'active');
