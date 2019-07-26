---
title: Notes on Making an Internal R Package for Team
author: Amy Tzu-Yu Chen
date: '2019-07-26'
slug: notes-on-making-internal-r-package-in-org-team
categories:
  - R
tags:
  - R
---

A month ago, Malcolm asked on Slack about how to make internal R packages for company/organization/team. I ended up summarizing some useful practices that I learned from System1 DS team. 

## The Conversation | June 26, 2019
Malcolm Barrett: Anyone have resources or best practices they like for making internal packages? ...

Amy Tzu-Yu Chen: I don’t really have any written resources but i learned some "better" practices while building internal packages with the team. I’ll try to write them down but really, I learned by reviewing Gergely and my other teammates’ codes

### What should be in the package?

First of all, an internal package is sth you build for *all R users* in your company. So it’s important to understand what they need. A lot of helper functions are not too fancy. They could be

- data formatter (convert to dollar, 2 or 4 digit precision etc. You could argue that we have those fns in existing R pkgs, but wrapping the useful ones into internal pkg could make less experienced useRs happy)

- reduce imports: I find it soothing when I can import the internal package and then all i need is magically in there. For example, if you `%>%` all the time, then export it to your internal pkg. If all your analyst has 10 lines of library(xxx) in all their R scripts, there’s probably room for improvement

- graph theme. Everyone uses ggplot and it looks “professional” when your company’s useRs use the same theme (you could customize theme in your company. there’re color-blind users at my company so we have a color-blind friendly theme)

- db helpers: probably the most used set of helpers at my job. The idea is that everyone at the company could run one single fn to get data from any internal db. This eventually led to the open-source package https://github.com/daroczig/dbr

- s3 or equivalent helpers: the use of s3 is very common. We read from and write to s3 all the time. This eventually led to the pkg https://github.com/daroczig/botor

- secret manager: you don’t want your secrets flying around the company. Otherwise, the pythonistas at your company can easily pick on your R codes. `botor::kms_decrypt` can help. Note that secret manager does not have to be passwords. It could also be other sensitive information in your company
- slack/google drive etc helpers: whatever your team likes to use to pass stuff around, make it easier and accessible in R

- make pkg accessible to all types of internal useRs: a simple example would be that your fn to query db automatically returns DT so `data.table` useRs don’t have to `setDT` all the time. My team has both “data.table” and “tidy” useRs

### Collaboration
Second, *code reviews* is important. Main useRs in the company should code review each other’s edits on the internal package and be a contributor.

### Be open-source minded
Third, design internal pkg to streamline your and your co-workers’ work processes, but it’s nice to be open-source minded. Ask yourself if you can open-source parts of your work and make it available to the public. https://system1.com/open-source is a result of being open-source minded

#### Disclaimer
I am mainly a user of these internal/open-source packages. Wanna attribute credits to Gergely
[@daroczig](https://github.com/daroczig) and Neal Fultz [@nfultz](https://github.com/nfultz) who made these happen in the first place. Follow them on Github to make them happy

