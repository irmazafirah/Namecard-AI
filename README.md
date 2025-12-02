## Node-RED Setup
1. Open Node-RED.
2. Download flows.json file and import in Node-RED.
3. Install Aedes MQTT Broker module and Webcam UI module.

## n8n Setup
1. Open n8n.
2. Download Namecard AI.json and import in n8n.
3. Setup credentials for each node.

### MQTT Trigger
> Protocol = Mqtt\
Host = \
Port = 1883\
Username = \
Password = \
Client ID =

### Read/Write Files from Disk
Change the image path.

### OpenAI
Get your own API Key.

### Google Sheets
1. Setup a project in Google Cloud Console.
2. Enable Google Drive API and Google Sheets API.
3. Get Client ID and Client Secret.
4. Specify the Google Sheet Document.
5. Choose the Sheet page inside the specified Google Sheet Document.
6. Map the columns manually.

> Name = {{ $json.Name }}\
Company = {{ $json.Company }}\
Job Title = {{ $json['Job Title'] }}\
Email = {{ $json.Email }}\
Primary Phone = {{ $json['Primary Phone'] }}\
Tel Phone = {{ $json['Tel Phone'] }}\
Fax Phone = {{ $json['Fax Phone'] }}\
Address = {{ $json.Address }}\
Nature of Business = {{ $json['Nature of Business'] }}

### Outlook
1. Register app in Microsoft Azure. This will be the account of email sender.
2. Get Client ID (Application (client) ID) and Client Secret (Value).
