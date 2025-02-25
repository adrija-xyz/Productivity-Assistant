# Productivity-Assistant
An AI-Powered Slack Bot: Optimize Your Workday, Protect Your Well-being

# BurnoutBot

**An AI-Powered Slack Bot: Optimize Your Workday, Protect Your Well-being**

## Inspiration
In today's remote work environment, calendar management has become increasingly challenging. We noticed that many professionals struggle with back-to-back meetings, lack of breaks, and poor work-life balance. We were inspired to create a solution that not only manages schedules but actively protects mental well-being.

## What it does
BurnoutBot is a Slack Bot that automatically detects meeting overload and schedules recovery breaks on Google Calendar. By reading users’ calendars, it flags potential burnout (e.g., excessive daily meetings or back-to-back sessions), then proactively suggests shorter meetings, combines overlapping appointments, and auto-inserts “No Meeting” blocks for recovery time. All interaction happens in Slack via simple commands

It helps teams manage their calendars more effectively by:
- Analyzing calendar health and providing burnout risk assessments
- Suggesting optimal break times between meetings
- Finding the best meeting slots for team collaboration
- Optimizing meeting schedules to prevent overload
- Providing team workload analysis and availability tracking


## How we built it
We built BurnoutBot using:
- **Node.js** for the backend
- **Slack Bolt API** for bot interactions
- **Google Calendar API** for calendar management
- **Firebase** for persistent token storage
- **OpenAI's GPT-4** for intelligent scheduling suggestions
- **Moment.js** for time management

The core scheduling logic uses algorithms to find optimal meeting times while considering everyone's workload and burnout risk.

### Available Commands
- **/calendar**: View your calendar events (supports 'week' and 'month' views)
- **/reschedule**: Get assistance in rescheduling your meetings
- **/workload**: Analyze your meeting workload with burnout risk assessment
- **/calendar-health**: Get a detailed health report of your calendar
- **/optimize-meetings**: Get smart recommendations for optimizing your meetings
- **/team-workload**: Shows total team meeting load
- **/team-availability**: Finds optimal meeting times for the whole team

## Challenges we ran into
1. **Token persistence:** Initially, users had to re-authenticate frequently. We solved this by implementing Firebase token storage.
2. **Complex scheduling logic:** Balancing multiple calendars while considering burnout scores required careful algorithm design.
3. **Time zone handling:** Managing meetings across different time zones needed precise datetime management.
4. **Meeting optimization:** Creating intelligent break suggestions while respecting existing schedules was challenging.

## Accomplishments that we're proud of
1. **Sophisticated burnout detection system**
2. **Intelligent team availability finder**
3. **Seamless Google Calendar integration**
4. **Real-time workload analysis**
5. **User-friendly Slack interface**

## What we learned
- Advanced calendar management algorithms
- Complex scheduling optimization
- Token management and authentication flows
- Team workload analysis techniques
- Integration of multiple APIs _(Slack, Google Calendar, OpenAI)_

## What's next for BurnoutBot
1. Machine learning integration to predict optimal meeting times based on past patterns
2. More detailed analytics and reporting features
3. Integration with other calendar platforms
4. Custom organizational policies for meeting scheduling
5. Advanced team productivity metrics
6. Personal productivity insights and recommendations

