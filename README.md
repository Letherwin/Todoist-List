# Todoist-List
Todoist Custom Card for Home Assistant - Lovelace

Basic Custom Card for Lovelace.
It lets you choose a calendar from todoist, and shows a list of tasks in that calendar.
You may choose a title for the Card.

Put todoist-list.js in your www directory.

Reference the file in ui-lovelace.yaml:

resources:
  - url: /local/todoist-list.js?v=1
    type: js

create a new card:

- type: 'custom:todoist-list'
      entity: calendar.some_calendar
      title: 'Some Title'
