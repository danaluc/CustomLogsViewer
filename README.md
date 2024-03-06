# Magento 2 Custom Log Reader Extension

## Description
This Magento 2 extension allows you to easily read log files from the Magento back office, including both standard Magento logs and any custom logs located in the var/log folder of your Magento installation.

## Features
- View standard Magento logs and custom logs from the Magento back office.
- Simplify tracking and issue resolution by accessing log files directly within Magento.

## Installation
1. Clone or download the repository.
2. Extract the contents into the `app/code` directory of your Magento 2 installation.
3. Run the following commands:

   ```bash
   php bin/magento module:enable Danaluc_CustomLogsViewer
   php bin/magento setup:upgrade
   php bin/magento setup:di:compile
   php bin/magento setup:static-content:deploy -f
   php bin/magento cache:clean

## Usage
1. Log in to your Magento back office.
2. Navigate to the log reader extension.
3. Browse and view log files as needed.

## Support
If you encounter any issues or have questions about this extension, please [open an issue](https://github.com/danaluc/CustomLogsViewer.git/issues) on GitHub.

## License
This project is licensed under the [MIT License](LICENSE).