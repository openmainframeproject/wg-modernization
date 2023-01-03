# [COMMUNITY NAME] Working Group Meeting - <%= date.toFormat("MMMM d, yyyy") %>

## Attendance

- [ ] Person A, Afflilation
- [ ] Person B, Afflilation
...

## Agenda

Extracted from **<%= agendaLabel %>** labelled issues and pull requests from **<%= owner %>/<%= repo %>** prior to the meeting.

<%= agendaIssues.map((i) => {
  return `* ${i.title} [#${i.number}](${i.html_url})`
}).join('\n') %>

## Action Items


## Notes

## Chat
