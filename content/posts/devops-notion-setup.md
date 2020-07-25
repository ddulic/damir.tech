---
title: DevOps Notion Setup 📝
date: 2020-07-25 16:10:22
images:
  - /img/background_notion.jpg
tags:
  - notion
  - jira
  - markdown
  - organisation
  - productivity
---

# Requirements
As a DevOps Engineer I had a problem I was looking to solve for a long time.

How to do productive work (be in the zone), take useful notes without getting distracted and transfer them in a readable way in a ticket tracking system like Jira.

A system was needed.

# Investigation
I played around with various tools in the past, here are just some of the things I tried:
- Plain Text Files
- Jupiter Notebooks
- Self Hosted Wiki
- Physical Notebooks
- Evernote

Some of them didn't work, some of them worked for a while, but none of them worked as well as [Notion](http://notion.so).

So here is my Notion work setup. This won't apply to everyone as each person's requirements are different.

You don't have to be DevOps to use this system, it can also be applied to other roles, anything that relates to inputting formatted text and code into a website like Jira.

# Solution
This system treats **tickets** are the source of truth. No task should be completed without a ticket, this is why everything references tickets and the main notes are kept in the tickets.

There are 2 main sections:
- Notes
- Log

## Notes
This is where you will be 90% of the time.

{{< figure src="/img/notion_notes.png" alt="notion_notes" class="big" >}}
Apologies for the truncation, you understand.

### Properties
![notion_notes_properties](/img/notion_notes_properties.png)


### Templates
![notion_notes_templates](/img/notion_notes_templates.png)

### Ticket Template
```text
# Information

## Meeting (template button)

Date: YYYY-MM-DD
Participants: <name>,


## Catchup (template button)

Date: YYYY-MM-DD
Participants: <name>,

Agenda:

- 

Todo:

- [ ] 

---

## Related

<link to page>

# Comments

# Tasks

- [ ]
```

As for the other templates, I think they are pretty self explanatory, so I won't be putting them here.

When I start working on a new ticket, I fill in the any information required for that ticket in the `# Information` section.

`## Meeting` and `## Catchup` are [template buttons](https://www.notion.so/Create-your-own-templates-5c033c12ac3b4c1fb4703491be74550d) which are only added if there is a related Meeting or Catchup related to the ticket.

`## Related` section is for any related tickets, linked as Notion page links if previously worked on, or normal links if they are not in Notion.

`# Comments` section is where it gets interesting. Each block within, separated by `---` is a comment on the ticket. These initially start out as a collection of scattered bullet points, code blocks, links and what ever else that is related to the current work being done.
End of day or when a block of work is done I go over the notes, make them readable and pretty before copying the section and pasting it as is to Jira, which now fully supports Markdown.
The only issue I have found so far is that I can't paste images that have been added to Notion... so I usually wait until the ticket is added to Jira before adding the image to both Jira and Notion, not a huge problem but indeed a small annoyance.

`# Tasks` is where all the action items related to the current ticket sit. This is an ever evolving section with actions constantly being added, removed and edited as the work progresses.
I usually keep this section cloned and synced to the ticket's description in Jira. If a ticket becomes to big, as can happen with a lot of investigation tickets, a section can be broken off into subtasks.

## Log
The remaining 10%.

{{< figure src="/img/notion_log.png" alt="notion_log" class="big" >}}
Again, apologies for the truncation, you understand.

### Properties
![notion_log_properties](/img/notion_log_properties.png)
`Property` points to a Note property (as can be seen in the above image).

### Templates
![notion_log_templates](/img/notion_log_templates.png)
`$NUM` is replaced by the week number (tracked since I started working at the company).

### Week Template
```text
### Monday

> 
- 

### Tuesday

>
- 

### Wednesday

>
- 

### Thursday

>
- 

### Friday

>
- 

---

### Weekend

- [ ]  
-
```

This is where the "logs" live. It shows me what work was done on a given day (useful for standups and progress updates) and what is coming up in terms of scheduled tickets and tasks.

Tasks part of a ticket are usually copy-pasted from the `# Tasks` section under a ticket note.

At the beggining of each day I take a look at the work that is scheduled to be completed that day and at the end of the day I make note of the work that was actually completed.

# Conclusion
This is only one part of my whole workflow.

I use a multitude of other tools as well as the [Notion Web Clipper](https://www.notion.so/Web-Clipper-ba54b19ecaeb466b8070b9e683c5fce1) extensively, mainly for bookmarks.

I will **not** be posting a Notion template as I find them pretty useless. Coping something someone else made doesn't make you think and understand how the system should look like. Idealy you would take the concepts of the system I use (if you agree with it) and create something that works best for you.

Thanks for taking the time to read.

Stay safe and have a great day!