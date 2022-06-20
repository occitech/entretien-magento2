# Entretien Magento 2

## Intro

This repository is intended to be as easy as possible to install for running a Magento on your local environment.
Meaning that you should never use it on environment accessible from outside your network since it use comited weak passwords.

We use this repository to deploy Magento and run technical test when a developper apply to a job at Occitech.

## Setup

* Get this git repository locally.
* Start docker project : `make start`
* Run composer install : `make composer install`
  * When prompt ask for credentials for `repo.magento.com`, put your Magento public key as Username and private key as Password, 
  * Then say `Y` to store these credentials in .composer/auth.json when you are asking for.
- Import DB : `make mysql < magento.sql`.
- Ajouter `127.0.0.1 magento.test` dans le fichier `hosts`.
- Check if everything runs fine (passwords are in `env/*.env`).
