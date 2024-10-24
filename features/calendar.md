# Calendar

## Overview
The Calendar feature allows users to view, manage, and explore events across different time frames (daily, weekly, monthly). It provides a user-friendly interface for scheduling and discovering events, enhancing the user's ability to stay organized with campus activities.

## Key Functions
- View the user’s events on a daily, weekly, or monthly basis.
- Add new events to the calendar.
- Explore events that are categorized by the user’s interests and tags.

## Usage
- **Main Calendar View**: Users can toggle between daily, weekly, and monthly views to see all the events scheduled for the chosen time frame. The interface allows users to scroll through days, weeks, and months to navigate past and future events.
- **Event Creation**: Users can create new events by clicking the "Create Event" button found in the ribbon section.
- **Event Exploration**: Users can explore various events through the Event Section, which sorts events based on the user's interest tags.
  
### Calendar Components:
- **<MainCalendar/>**: Displays the monthly, weekly, and daily views, showing the user’s events for the selected time frame.
- **<RibbonComponent/>**: Contains buttons to create a new event and toggle between calendar views (monthly, weekly, daily).
- **<MiniCalendar/>**: Displays the current month with visual indicators for the current day and days with events.
- **<EventSection/>**: Contains a list of events separated by those that match the user’s tags and those that don’t.
  
### Other Components:
- **<CalendarDay/>**: Displays the day number and any events scheduled for that day.
- **<CalendarMonthView/>**: Displays the entire month with days showing their events.
- **<CalendarWeekView/>**: Displays the current week, showing events for each day.
- **<CalendarDayView/>**: Displays the events for the selected day.

## Examples (Optional)
- A user can view the entire month’s events using the monthly calendar view, or switch to a daily or weekly view for a more detailed look at scheduled events.
- Users can add new events by clicking the "Create Event" button in the ribbon and filling in event details.

## Additional Notes (Optional)
The calendar feature integrates with the user’s profile to display personalized events based on tags and interests, ensuring that relevant campus activities are highlighted.

---

# Component Reference

## How to Add to This Reference
When a new component is created, add a new line at the end following this format. Include the component's name with a link to its documentation and a brief description.

### Existing Components:

#### <MainCalendar/> - Contributors: cseba11, ggonza28, Ojani, SammyAlva04, vivianaramos6
Displays the monthly, weekly, and daily views of events, allowing users to scroll through dates to view past and future events.

#### <RibbonComponent/> - Contributors: cseba11, GabyMarr, Ojani, SammyAlva04, vivianaramos
Contains controls for toggling between calendar views and creating new events.

#### <MiniCalendar/> - Contributors: cseba11, GabyMarr, Ojani, SammyAlva04, vivianaramos
Displays a miniature version of the calendar, highlighting the current day and marking days with events.

---

## Contributors
- **cseba11**
- **ggonza28**
- **Ojani**
- **SammyAlva04**
- **vivianaramos6**
- **GabyMarr**
