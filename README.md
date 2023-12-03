# Track Zone

## Requirements

- User can set their own time and timezone, this clock can't be deleted only be edited
- User can create as many clock as they want
- Each clock has their own title or name
- Own Timezone
- Simple Events with time
- Time difference between users timezone and clock timezone in hour and minute
- User can edit or delete a clock
- Timezone could be UTC (standard), GMT, PST, EST
- only date-ns library is allowed for this project. rest of the logic should write by yourself
- Every data must be validated

## Requirements Breakdown

- We will have a local clock and a list of clocks
- We will create the initial clock from user timezone
- Clock object will look like
  - id
  - title
  - timezone
    - type (UTC, GMT, PST, EST)
    - offset (Only for UTC and GMT)
  - events
- Event object will look like
  - id
  - text
  - clockId
  - timezone
  - startTime
  - endTime
- We will use a clock object for local clock
- Use an array of clocks for other clocks
- We will use event id to create events inside clock

### Clock Features

- properties
- update clock
- delete clock
- calculate difference
- update events

### Event Features

- properties
- create event
- delete event
- update event
- filter event by clock
- get event by id
- get events by ids

## Component Tree

### App Component

![app.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361105359/qYcHsXUfO.jpg)

### Reusable components

![shared.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361210554/Enxr__Lh3.jpg)

### UI Components

![ui.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361295889/xZp23vZgg.jpg)

### Clock Display Component

![clock-display.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361350686/NJGDn-2CR.jpg)

### Clock Form Component

![clock-form.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361406489/EmwuVPdmE.jpg)

### Clock Actions Component

![clock-actions.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361479586/i1H4iQ9XJ.jpg)

### Create Event Form Component

![create-event-form.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361528283/656X1EuAB.jpg)

## Hooks

![hooks.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361563559/jV4KNrNwN.jpg)

## Data Flow

![data-flow.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1666361597873/57EMROBND.jpg)
