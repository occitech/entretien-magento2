#### Setup

* Get this git repository locally.
* Start docker project : `make start`
* Run composer install : `make composer install`
** When prompt ask for credentials for repo.magento.com, put your Magento public key as Username and private key as Password, 
** Then say `Y` to store these credentials in .composer/auth.json
- Import DB : `make mysql < magento.sql`
- Disable 2FA authentication :  `make n98-magerun2 module:disable Magento_TwoFactorAuth`
- Check if everything runs fine (password are in env/*.env).