HOla !
Code version : beta
Opencart version : 1.5.4

before you upload the code to server 

Fellow these steps
* since am using dob(date of birth) as a case study, you can just replace dob to any name you prefer.
* Go to to Phpmyadmin section in your database.
* Select the the database name
* click on sql button at the top end
* Paste this code:

ALTER TABLE `customer` ADD `dob` DATE NULL AFTER `email`

press the go button.

after that  paste this also

ALTER TABLE `order` ADD `dob` DATE NULL AFTER `email`

press the go button.


NOTE: if it seems like nothing is working check these two file.
- system => logs => error.txt
&

- vqmod => vqcache 'select any file depending on where the error is coming from'
- Vqmod => logs =>  'select any file depending on day you are currently working'