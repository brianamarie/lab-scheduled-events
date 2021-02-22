# Welcome to the scheduled events lab!

This lab is an exercise to check your knowledge on scheduled events. It is automatically graded via a workflow once you have completed the instructions.

**Quick links:**
- [About this lab](#about-this-lab)
- [Instructions](#instructions)
- [Seeing your result](#seeing-your-result)
- [Troubleshooting](#troubleshooting)
- [Useful resources](#useful-resources)

## About this lab

:warning: A grading script exists under `.github/workflows/grading.yml`. You do not need to use this workflow for any purpose and **altering its contents will affect the repository's ability to assess your lab and give feedback.**

:warning: This lab utilizes [GitHub Actions](https://docs.github.com/en/actions), which is free for public repositories and self-hosted runners, but may incur charges on private repositories. See *[About billing for GitHub Actions]* to learn more.

:information_source: The use of GitHub actions also means that it may take the grading workflow a few seconds and sometimes minutes to run.

## Instructions

In the `.github/workflows` folder of this repo, you'll find 3 workflows which we describe below with their intended purpose. Each workflow is complete **except for** the `on:` key.

- `stale-daily.yml`: checks for stale issues daily at midnight and closes them
- `stale-weekly.yml`: checks for stale issues every Monday and closes them
- `stale-monthly.yml`: checks for stale issues on the first of every month and closes them

Please complete the instructions below:
1. Create your own copy of this repository by using the [Use this template](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template#creating-a-repository-from-a-template) button.
2. In your newly created repository, create a new branch.
3. On your new branch, edit the `on` key of each `stale` workflow so that:
    - `stale-daily.yml` contains a trigger to run daily at midnight
    - `stale-weekly.yml` contains a trigger to run every Monday
    - `stale-monthly.yml` contains a trigger to run on the first of every month

## Seeing your result

Your lab is graded automatically once you have completed the instructions. To see the result of your lab, click the **Actions** tab, select the **Grading workflow**, and select the most recent workflow run. The status of the workflow indicates if you have passed or failed the lab.

If the workflow failed, scroll down to the **Annotations** section to check what went wrong.

See *[Viewing workflow run history]* if you need assistance.

## Troubleshooting

 If the grading workflow does not automatically run after you complete the instructions, run the troubleshooter: in the **Actions** tab select the **Grading workflow**, click **Run workflow**, select the appropriate branch, and click the **Run workflow** button.

See *[Running a workflow on GitHub]* if you need assistance.

## Useful resources

Use these to help you!

Resources specific to this lab:
- [Events that trigger workflows - GitHub Docs]
- [Cron examples - Crontab.guru]

Resources for working with labs and GitHub Actions in general:
- [Creating a repository from a template]
- [Viewing workflow run history]
- [Running a workflow on GitHub]
- [About billing for GitHub Actions]
- [GitHub Actions]


<!--
Links used throughout this README:
-->
[Events that trigger workflows - GitHub Docs]: https://docs.github.com/en/free-pro-team@latest/actions/reference/events-that-trigger-workflows#schedule
[Cron examples - Crontab.guru]: https://crontab.guru/examples.html
[Creating a repository from a template]:                        https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template
[Viewing workflow run history]:                                 https://docs.github.com/en/actions/managing-workflow-runs/viewing-workflow-run-history
[Running a workflow on GitHub]:                                 https://docs.github.com/en/actions/managing-workflow-runs/manually-running-a-workflow#running-a-workflow-on-github
[About billing for GitHub Actions]:                             https://docs.github.com/en/github/setting-up-and-managing-billing-and-payments-on-github/about-billing-for-github-actions
[GitHub Actions]:                                               https://docs.github.com/en/actions
