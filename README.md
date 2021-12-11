# SSID-QR-code-generator
Creating a QR code for your Wifi to connect to your wifi instantly.

Install-Module QRCodeGenerator -Scope CurrentUser -Force

$wifi = 'SSID' #name of the Wifi Network to be added in teh QR code
$path = 'c:\temp\QRCode 5GHz.png' #define location for QR code generated
$pwd = 'Wifi Password' #password for the SSID mentioned above


New-QRCodeWifiAccess -SSID $wifi -Password $pwd -OutPath $path
