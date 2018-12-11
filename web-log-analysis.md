# Web Server Logs
Often contain access and error logs.

Database services will also have logs.

## AW Stats
Open source log analyzer.

Uses PERL for it's operation as PERL is the gold standard for text manipulation libraries.

## Apache
Log location dependant on OS
> Set in `httpd.conf`

Some settings:
* LogLevel
  * levels of reportings.
  * Most systems runn in notice, warn, or error mode.
    * Notice or warn for dev. Error for production.
    * Changes require server restart.

## IIS

Logs often found in `C:\inetpub\logs`.

Files can be binary so may require aditional config.

Configured through `IIS Management Console`.

## AWStats: The Arbitrary Second Section

* Can be dynamic or one-off
* conf file must be configured for the job.
* Best if it can be copied to the xampp folder.

## Running AWStats
Must specify log file location.
Required running `awstats.pl` command.

I'm pretty sure the rest of the notes are just cruft and unimportant for the test.