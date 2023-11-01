# Project 7 - *Get It Done*

Submitted by: **Nick Alarcon**

**Get It Done** is an app that ... [TODO] 

- Allows users to create and update tasks and are saved to User defaults(local storage)
- User can add a title, description and due date and time for task, as well as priority
- User can mark the task as done, which grays it out. Otherwise task are sorted by due date and priority
- User can edit task by tapping on it and also can delete task by swiping left
- Allows user to view task by date in calendar view and mark them done, and also view priority
- Sends a user notification (if user accepts notifications) about any given task due in 5 mins

Time spent: **12** hours spent in total

## Required Features

The following **required** functionality is completed:

- [x] App displays a list of tasks
- [x] Users can add tasks to the list
- [x] Session persists when application is closed and relaunched (tasks dont get deleted when closing app) 
- [x] Note: You have to quit the app, not minimize it, in order to see the persistence.
- [x] Tasks can be deleted
- [x] Users have a calendar view via navigation controller that displays tasks    


The following **additional** features are implemented:

- [x] Tasks can be toggled completed
- [x] User can edit tasks by tapping on the task in the feed view
- [x] User can add priority tag to task (Low, Medium, High)
- [x] User can add time due for task
- [x] Tasks sorted by due date and priority
- [x] Current tasks show time its due and priority
- [x] Tasks in Calendar View show priority tag
- [x] Added user Notifications for 5 mins before task is due
- [x] Time due changes color based on proximity of due time (1 hr: Red, 4 hr: Orange, 24 hr: Green)
- [x] Updated theme to support dark mode
- [x] Updated UI with different tint and font
- [x] Added custom app logo

## Video Walkthrough

<a href="https://www.loom.com/share/18b346de1645430e9db6f87790239d31">
      <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/18b346de1645430e9db6f87790239d31-with-play.gif">
    </a>

## Notes

Building this app has been one of the more funner projects I have completed for this course. While setting the initial required features was simple enough, I took creative liberty to transform this app by adding more productivity features but also keeping the app simple and quick for users. Since most of the functionality had been implemented already, I took the time to read through the documentation and really think of features to add. One of the features that took the longest to implement was adding the priority tag for tasks. The reason this took a while to implement was because I had to edit the different files to contain the priority information (Task, TaskCell) and also add the associated label in the TaskListViewController and CalendarViewController. Additionally, I had to adjust the sorting logic to take into account the priority of the task.
Additionally, another feature that I thought would really add to the app was implementing notifications. This process was actually more simple, which required editing AppDelegate to ask the user for notification permissions. Then I updated my logic to incorporate the time it was due and therefore schedule a notification 5 minutes before the task is due. Although the notification does not apepar in the simulator, I tested this on my personal device and the notification does work. In the future, I hope to continue developing this app by adding reoccuring tasks and modifying the notification system to send various alerts a diffrent time periods. Furthermore, the next feature I plan to add is a segue inside the the CalendarView which presents a view of the different time periods for a single day so it shows user the diffrerent tasks at different time periods for one day.

## License

    Copyright [2023] [Nick Alarcon]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
