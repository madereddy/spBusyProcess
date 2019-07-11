# spBusyProcess
This script will catch all long running queries in user databases that run over the allotted @KillTime and kill them. It will also send email alerts to whoever is specified.

## Getting Started

Run spBusyProcess against the master database to create the stored procedure.

### Usage

Run EXEC spBusyProcess @KillTime = 1, @EmailAddress = 'admin@madereddy.com', @MailProfile = 'Default'

This command will kill any process running over a minute and email admin@madereddy.com with the mail profile Default.

## Authors

* **Aasim Abdullah** - *Initial work* - http://connectsql.blogspot.com
* **madereddy**- *Stored Procedure and Parametrization*

## Acknowledgments

The base of the script is from Aasim Abdullah. This is his website http://connectsql.blogspot.com
