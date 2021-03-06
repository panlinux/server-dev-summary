# Ubuntu Sever Development Summary

This repository is used by the Canonical Server team to develop the weekly
development summary that is sent out to the community as a whole. This summary
is used to communicate accomplishments and progress made by the server team
over the previous week.

## Template

The template is a starter to generating the weekly summary. This is used to
allow whoever is working on the summary to focus on content and not style.

## Instructions

Below is a list of steps to generate the complete summary:

1. Ubuntu Server Image
    - [Go create it](https://docs.google.com/presentation/d/10Jj-Qyu1OMhwtijCgZrKqiF4z6Z4NOeT5opowyq6Mew/edit?usp=sharing)
1. Template & Uploads
    - Run the `generate.sh` script to create a new markdown file for today and
      base it off of deltas between the most recent previous report's date
1. cloud-init and curtin
    - Review the Trello board done column
    - Summarize any done cards and add any missing items to the auto-generated
      items
1. Ubuntu Server
    - Review the Trello board done column
    - Summarize any done cards and add any missing items to the auto-generated
      items
1. Review
    - Send out a link to the draft for review to the team
    - Check spelling and grammar during this time as well
1. Run `publish.sh` to generate html and email formats
1. Insights
      1. Login to admin.insights.ubuntu.com/login and create new post
      2. Create new blog post: articles -> add an article
      3. Title: "Ubuntu Server development summary - DD Month YYYY"
      4. Tags: Ubuntu Server, Server, weekly
      5. Topic: Cloud, Server
      6. Group: Cloud and server
      7. Text Tab: Paste html from chrome app
      8. Bottom Right: Featured Image -> Set Featured Image
      9. Publish!
1. Discourse
      1. Login to server hub at https://discources.ubuntu.com/c/server
      2. Click new topic button 
      3. Title: "Ubuntu Server development summary - DD Month YYYY"
      4. Click the 'Upload' button above the text area for the new topic and upload the same png image you created for the insights post
      5. Paste the html output used in insights step above.
1. Send email to ubuntu-server
    - Use the $date.email file as the body of the email
    - Subject: Ubuntu Server development summary - DD Month YYYY
    - to: ubuntu-server@lists.ubuntu.com
    - bcc: lwn@lwn.net
1. Announce
    - Announce the post in #marketing about the post
