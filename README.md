# Paystack OpenCart Extension

## Description
OpenCart Paystack payment gateway integration. Visit the [Paystack Website](http://paystack.com) to know how paystack works.
Install to receive payments for your goods in naira from any Mastercard, Visa or Verve card in the world.

## Requirements
- Curl 7.34.0 or more recent
- PHP 5.5.19 or more recent
- OpenSSL v1.0.1 or more recent

## Notes
- Paystack currently only accepts the following currencies: `NGN`, `USD` and `GHS`.
- You need to have created an account on [paystack.com](https://dashboard.paystack.co/#/signup).

## Features:
- Paystack payment gateway integration
- Activates payment module only when cart currency is `NGN`, `USD`or `GHS`.
- Activate payment module only when order total reaches the amount you specified
- Captures call back notification to automatically update order status
- Simply turn on Live Mode to accept live payments.

## Installation
0. Visit [Paystack OpenCart Extension](http://www.opencart.com/index.php?route=extension/extension/info&extension_id=25767&filter_search=paystack) to download the latest release.
1. Unzip the files. Select the right version for your OpenCart.
2. Upload the files to your OpenCart installation folder with a FTP client 
                     `OR`
3. Upload the zipped file to the root of your OpenCart installation then unzip using cPanel File Manager. The folders should merge. 
4. In admin panel, proceed to ‘Extensions > Payment’ and install ‘Paystack’.
5. Configure the module accordingly. 
 - To get your live and test secret keys, visit [the Paystack Dashboard](https://dashboard.paystack.co/#/settings/developer).
6. Enable Paystack payment gateway on your OpenCart admin.
7. Add and set NGN, GHS or USD as your default store currency.
8. Proceed to [Paystack OpenCart Extension](http://www.opencart.com/index.php?route=extension/extension/info&extension_id=25767&filter_search=paystack) to rate our work.

## Running the paystack OpenCart plugin on docker
Contained within this repo, is a dockerfile and a docker-compose file to quickly spin up an opencart and mysql container with the paystack opencart plugin installed.

### Prerequisites
- Install [Docker](https://www.docker.com/)

### Quick Steps
- Create a `local.env` file off the `local.env.sample` in the root directory. Replace the `*******` with the right values
- Run `docker-compose up` from the root directory to build and start the mysql and opencart containers.
- Visit `localhost:8000` on your browser to access and setup opencart.
- Run `docker-compose stop` from the root directory to stop the containers.

## Other Configuration
To add currencies, you can do so at System > Localisation > Currencies. 

## Documentation
* [Paystack Documentation](https://developers.paystack.co/v2.0/docs/)
* [Paystack Helpdesk](https://paystack.com/help)

## Support
For bug reports and feature requests directly related to this plugin, please use the [issue tracker](https://github.com/PaystackHQ/plugin-opencart-3.x/issues). 

For general support or questions about your Paystack account, you can reach out by sending a message from [our website](https://paystack.com/contact).

## Community
If you are a developer, please join our Developer Community on [Slack](https://slack.paystack.com).

## Contributing to OpenCart Extension for Paystack

If you have a patch or have stumbled upon an issue with the OpenCart extension for Paystack, you can contribute this back to the code. Please read our [contributor guidelines](https://github.com/PaystackHQ/plugin-opencart-3.x/blob/master/CONTRIBUTING.md) for more information how you can do this.
