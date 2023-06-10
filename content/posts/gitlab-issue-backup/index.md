+++
author = "Matt Lilley"
title = "Backup Gitlab issues"
date = "2023-05-04"
description = "My brain suddenly surfaced those immortal 3 letters... GPT 🤩 and that's when I knew the way I worked was going to change. I was blown away by the quality and completeness of the code that GPT4 created."
subtitle="My first GPT 💡 moment"
tags = [
    "technology",
    "gpt"
]
+++

If you followed my [cold fusion series]({{< relref "/series/cold-fusion-lenr" >}}), then you'll know that I built my own reactor and did some experiments over the course of 2018-2020. Back then, I decided to write my experimental log using [issues on the lilley-lenr GitLab repository](https://gitlab.com/mklilley/lenr/-/issues). Each issue would be associated with an experimental campaign and each comment on an issue would contain a log of what I did that day. The issues worked quite nicely with the repo itself - which stored experimental data and analysis code.

Today, it struck me that I don't have a backup of my experimental log and, although it seems unlikely that GitLab will suddenly cease too exist, I would be distraught if I lost this data. After trawling through my hard drive, I found reference to repo I made called `gitlab-issues-backup` 🙌 . However, upon closer inspection I found but a single file containing:

```
// TODO:
// 1. get issues using https://gitlab.com/api/v4/projects/14183708/issues/
// 2. save the json response to disk as lilley-lenr-issues.json
// 3. loop through array to find the iid's of issues
// 4. get notes from issues using https://gitlab.com/api/v4/projects/14183708/issues/:iid/notes
// 5. save the json response to disk as lilley-lenr-issues-:iid-notes.json

```
🤬 not cool Matt... not cool!

Now, I know the tasks in this little todo list aren't that hard, but I've not been in API mode for a while and I know from experience that doing these simple things right does actually take quite a bit of time and... I'm just such a busy person at the moment 💅😉.

While wrestling with the inevitable, my brain suddenly surfaced those immortal 3 letters... GPT 🤩 and that's when I knew the way I worked was going to change. With these 4 prompts and 10 mins of implementing it was all done:

>Hi Geep. I'd like to write a node application that uses the gitlab api to backup issues that are associated with a specific repo that I own and also the comments/notes associated with the issues. Can you help me with that please?

...

> Thanks. Can you please implement pagination for the fetchIssueComments function?

...

> Thank you so much! Quick one, how do I get the project_Id from the repo?

...

> This is amazing thank you

Ok technically I didn't need prompt number 4, but being nice doesn't cost you...unless you're using GPT4 I guess 🤔.

I was blown away by the quality and completeness of the code that GPT4 created. You can take a look at the code on the [gitlab-issues-backup](https://github.com/mklilley/gitlab-issue-backup) repo on Github (GPT wrote 95% of this). Although it's only a small amount of code, I've got a feeling that GPT can do a lot more and I'm sure my brain is going to start finding lots of opportunities for me to test this out.


