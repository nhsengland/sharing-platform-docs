# Pretty Date
## When this pattern is used

When a platform user is viewing a group, dates will be displayed in pretty date format.  Exceptions to this such as user registration date will be defined within individual user stories.

## How this pattern is used

If the date relates to something that happened (eg a forum post) it will be displayed as follows:

* less than 60 seconds ago: 'Just now'
* Between 60 seconds and 90 seconds: '1 minute ago'
* Between 90 seconds and 60 minutes: '{minutes} minutes ago' where {minutes} is the number of minutes.
* Between 61 minutes and 120 minutes: '1 hour ago'
* Between 120 minutes and 24 hours:  '{hours} hours ago' where {hours} is the number of hours.
* Between 24 hours and 48 hours: 'yesterday'
* Between 48 hours and a 7 days: '{number of days} days ago' where {number of days} is the number of days. 
* Between 7 days and 31 days: '{number of weeks} weeks ago' where {number of weeks} is the number of weeks.
* More than 31 days: the date of the activity in the format dd month yyyy eg 18 February 2021


