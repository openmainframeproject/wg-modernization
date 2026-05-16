# Instructions for using this template

1) Review and update (README.md) with the working group name, and other details as approved by the TAC
2) To enable creating meeting agendas from GitHub issues, follow steps 3-5.
3) In the [meeting agenda template](.github/ISSUE_TEMPLATE/meeting.md), update `[COMMUNITY NAME]` and add the working groups members under the ['Attendance' section](.github/ISSUE_TEMPLATE/meeting.md#attendance).
4) Set the meeting date and time, along with the cadence in the [build agenda workflow](.github/workflows/build_agenda.yml) in the key `schedules:` that specifies a ISO-8601 interval. 
5) In the [send agenda workflow](.github/workflows/send_agenda.yml), update `[COMMUNITY NAME]` and `[MAILING LIST EMAIL]`. 
6) Any items with the label `meeting` will be added to the agenda automatically when it is built the day prior to the meeting.
