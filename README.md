# Speedtest dashboard widget for pfSense

## Install

Navigate to the command prompt ` Diagnostics > Command Prompt ` 

Issue the following command to install the speedtest package
```
pkg update ; pkg install -y $( pkg search speedtest-cli | awk '{ print $1 }' )
```

Copy the widget file **speedtest.widget.php** to **/usr/local/www/widgets/widgets/** with the following command.
```
curl -LJ https://raw.githubusercontent.com/jacobdjwilson/pfsense-speedtest-widget/master/speedtest.widget.php -o /usr/local/www/widgets/widgets/speedtest.widget.php
```

Install the widget on your dashboard through the web interface.
