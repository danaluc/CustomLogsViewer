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
2. Navigate to ***Store > Configuration > Danaluc > Custom Logs Viewer***.
3. Add General settings.
    
    - Configure Cron Schedule for cleanning logs: This option allows you to configure the cron options that establish the frequency with which each of the log files is checked for cleanliness. 
    - Custom Logs Files: Add all log files you need, remember log files must to be in `<Magento Root Dir>/var/log/`. Let column *Restart file every x days* empty if you don't want log files will be cleaned by schedule (cron). 

## Support
If you encounter any issues or have questions about this extension, please [open an issue](https://github.com/danaluc/CustomLogsViewer/issues) on GitHub.

## License
This project is licensed under the [MIT License](LICENSE).