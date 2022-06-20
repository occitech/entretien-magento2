#### Setup

- Get this git repository locally.
- Start docker project : make start.
- Import DB : make mysql < magento.sql
- Disable 2FA authentication :  `make n98-magerun2 module:disable Magento_TwoFactorAuth`
- Check if everything runs fine.