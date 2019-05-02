# [Daily] Handover Meeting Template

### Purpose

Our team follows the clock to maintain the Fedora and CentOS properties. 
Every day we meet to be sure that the following work continues from shift to shift:
- work in the datacenters (coordinating with remote hands)
- incidents
- community tasks that need to be completed before the responsible member's next shift

This lets us each go home for the evening, confident that important items are handled while we're away. 

### Anti-purpose

This is not a **personal status** or **planning** meeting, those activites happen at:
- The bi-weekly ticket grooming meeting (planning) `TODO: Add a link`
- Via email to the CPE list (status) `TODO: Add a link`

We should not be discussing priorities, grooming tickets, or discussing detailed procedures during this meeting.

### Attendees
| Attendee| Required? |
|-----|-----------|
| NA/SA Infra coordinator | Required | 
| EMEA Infra coordinator | Required |
| CPE Infra Team members | Optional |
| Community Members| Welcome | 

This meeting is relevant only to team members that have work that needs to be continued between shifts, 
which means team members without such tasks are not required to attend. If a responsible party is unable
to attend the meeting, they should summarize to the closest infra coordinator for reporting into the meeting.

#### Location
This meeting is held every day on IRC (`TODO: where?`) and is hosted by the 2 geo-coordinators 

## Agenda and minutes (Timeboxed to 15 minutes)
### Ongoing Issues (Clock 0:00)
This section is for things that infra members on the next shift should be aware of, but do not qualify as incidents.
Format: `[reporter/responsible member] description (link to report from the community if applicable)`
#### Fedora
* EXAMPLE: [bstinson] I'm noticing lots of extra load on foo.bar.ci.centos.org which runs some of the Fedora CI processes, please keep an eye on it
* EXAMPLE: [nirik] httpd is using a bunch of memory sometimes, when it does that please restart the service
#### CentOS
* EXAMPLE: [arrfab] The spammers are back on buildlogs, I've been rate limiting, and things seem to be holding

### Incidents and Maintenance (Clock 0:05)
This section is for outages that were completed, are ongoing, or will come up in the next shift
Format: `[person-assigned] Short description (link)`
- EXAMPLE: [cverna] We're upgrading openshift during this shift (http://link-to-taiga/ticket)
- EXAMPLE: [bstinson] Duffy ran out of nodes in CentOS CI (http://link-to-incident/email)

### Handovers (Clock 0:10)
This is for ongoing work in the datacenters or other tasks that need to be done.

- EXAMPLE: [bstinson -> arrfab] Network config on Rack C06 pending with DevOps
- EXAMPLE: [rick -> patrick] Config for foo needs to be done before tomorrow, I'm 3/4 done (link)

### Bye (Clock 0:15)
