# SendGrid Email Build/Release task
This build/release task can send emails via SendGrid **including attachments**.

## Prerequisite
You need to have a SendGrid Account created with an appropriate plan (they also have a free plan).
After you have an account you need to create an API key which can be easily done via the web interface from SendGrid.
This API key is needed in the build/release task.

# Configure SendGrid Section
The Sendgrid section contains the following fields:
* SendGrid Key (Required): API Key given by SendGrid. You can generate an API Key from the SendGrid Portal.


# Configure Mail Section
The Mail section contains the following fields:
* **To Address** (Required): To Addresses. Separated by commas (,).
* **Cc Address** (Optional): Cc Addresses. Separated by commas (,).
* **From Address** (Required): From Address.
* **Mail Subject** (Required): The subject of the email.
* **Html Body** (Required): The (html) body of the email.
* **Add Attachment** (Optional): Should be true in case you need to add an attachment.
* **Attachment** (Optional): Absolute path of the attachment.


# Release notes

1.2 | 21-10-2019
* Migrate to azure-pipelines-task-lib/task NPM package
* Fix issue when sending attachment from Windows agent

1.1 | 8-3-2019
* Support multiple addresses
* Add CC address

1.0 | 7-3-2019: Initial version


# Authors
* Jean-Pierre Broeders


# License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/CitrusAndriessen/tfs-mail-sendgrid/blob/master/LICENSE) file for details.