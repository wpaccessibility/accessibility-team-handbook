# Accessibility-ready theme testing instructions 

The purpose of this document is to provide instructions for `accessibility-ready` theme testing started during a contributor day.

The accessibility-ready requirements for themes are listed in the [Accessibility-Ready Requirements](https://wpaccessibility.org/docs/accessibility-ready/theme-guidelines/) section.
The section [Set up testing for the WordPress themes accessibility-ready program](https://wpaccessibility.org/docs/accessibility-ready/testing-themes/) outlines the steps for conducting a theme accessibility-ready requirements review.

## WordPress account

To contribute, you need to create an account on WordPress.org. This allows you to provide feedback to theme developers in Trac. Trac is the ticketing system for WordPress pre-GitHub, and how we communicate with theme developers.

Optionally, join Make WordPress Slack to participate in accessibility channels and ask questions while testing.

If you do not already have these accounts, please follow these steps:

1. Create a WordPress account at [login.wordpress.org/register](https://login.wordpress.org/register).
2. Join Slack at [make.wordpress.org/chat](https://make.wordpress.org/chat/).

If you have any questions while testing, please post them in the #accessibility-testing channel in WordPress Slack.

![Screenshot of Slack, with accessibility-testing highlighted in the menu bar.](https://make.wordpress.org/accessibility/files/2026/07/accessibility-testing-slack-channel.png)

## Contributor Day tasks

There are three key tasks that need to be completed during a Contributor Day. The following section describes those tasks and how you can help.

### Task 1: Assess and Action "Needs Report Review" Reports

Instructions:

1. Go to the [2026-05 Accessibility-Ready Theme Recheck Sheet](https://docs.google.com/spreadsheets/d/1uvT5ZyfAtwZGB4Hn8dfLE38lMmf55plKW1_QwPysg7A/edit?pli=1&gid=69736821#gid=69736821&fvid=998460810).
2. Above the table, click the "Views" button and select the "Group by Status & Sort by Last Updated (Most Recent First)" view.
3. Go to the themes with Status: Needs Report Review.
4. Select a theme to review and write your WordPress username in the notes column so everyone else knows you're reviewing it.
5. Click the link in the Report URL column to open the Google Sheet report.
6. Look at the Google Sheet report and see if there is enough information about failures to provide helpful feedback to the theme developer. Here is an [example comment with "enough information"](https://themes.trac.wordpress.org/ticket/263938#comment:2). Basically, you're looking for at least 3-4 concrete issues that can be shared with the developer.

If there is enough information:
1. Change the status from in-progress to failed.
2. Click the link in the "Latest Trac Ticket" column to go to Trac.
3. Post a comment for the developer on the Trac ticket, using the "If the theme has been tested" message template below and filling in information as applicable from the report.
4. Check the box in the "Message posted for theme dev" column.
5. Move on to another theme.

If there is not enough information:
1. Change the status from in-progress to P1 Needs Testing.
2. Delete the username in the "Tested by (dot org username)" column.
3. If you're willing, test the theme following the P1 Testing instructions below. If not, move on to another theme.

### Task 2: Test P1 Themes

Themes with a status of "P1 Needs Testing" are themes that are visible in WordPress.org theme search results because they have been updated in the last two years. 

Instructions:

1. Go to the [2026-05 Accessibility-Ready Theme Recheck Sheet](https://docs.google.com/spreadsheets/d/1uvT5ZyfAtwZGB4Hn8dfLE38lMmf55plKW1_QwPysg7A/edit?gid=69736821#gid=69736821&fvid=998460810)
2. Above the table, click the "Views" button and select the "Group by Status & Sort by Last Updated (Most Recent First)" view.
3. Go to the themes with Status: P1 Needs Testing.
4. Choose a theme to test, and:
   - Add your WordPress.org username in the tested by column.
   - Change the status to "In-progress".
5. Follow the instructions in [Getting set up to test](https://wpaccessibility.org/docs/testing/testing-themes/setup/):
   - Create a testing site on InstaWP or use a local install of WordPress.
   - Install and configure the theme.
   - Create your reporting spreadsheet (unless one already exists).
6. Add the links to your reporting sheet and your testing site in the "2026-05 Accessibility-Ready Theme Recheck" sheet (Report URL and Test URL columns).
7. Test your selected theme as described in the [accessibility-ready guidelines](https://wpaccessibility.org/docs/topics/theme-guidelines/), filling in the reporting sheet as you go.   
  **Important:** test until you find 3 or 4 failures, then stop and move on. See "Stop Testing Early" below.

If there are failures after testing:

1. Change the status from in-progress to failed.
2. Click the link in the "Latest Trac Ticket" column to go to Trac.
3. Post a comment for the developer on the Trac ticket, using the "If the theme has been tested" message template below and filling in information as applicable from the report. See example comment.
4. Check the box in the "Message posted for theme dev" column.

If there are no failures after testing: change the status from in-progress to passed.

#### Video Tutorial

If it helps you to watch a video of the demo site setup, report creation, and tips for testing, see this video, [How the New WordPress Accessibility Ready Testing Process Works](https://www.youtube.com/watch?v=XR-bZWqtr5s) on YouTube.

#### Stop Testing Early!

There are many themes to test, and we appreciate your time as a volunteer tester. We don’t expect you to spend hours testing a theme and reporting in detail failures on every row of the spreadsheet.

It’s ok to document representative issues, stop testing, and share the already identified failures with the theme developer, requesting fixes before you continue testing.
If you quickly identify multiple failures, such as:

* Missing skip links.
* Broken keyboard navigation.
* Color contrast failures.
* Empty buttons or links.
* Problems that are easily identified with Accessibility Checker or a browser extension.

**Stop testing** and give feedback to the developer.

### Task 3: Post Message for P2 Themes

Themes with a status of "P2 Needs Testing" are themes that were historically* not visible in WordPress.org theme search results because they have not been updated in the last two years. Ideally, all themes will get manually tested, but if there is not enough time for manual testing, posting a notice is better than nothing.

**Note on "historically"**: these themes are hidden if you first filter by the tag, but we discovered on June 3, 2026, that if you first click "latest" then filter by the tag all 268 of these themes will appear.

Instructions:

1.   Go to the [2026-05 Accessibility-Ready Theme Recheck Sheet](https://docs.google.com/spreadsheets/d/1uvT5ZyfAtwZGB4Hn8dfLE38lMmf55plKW1_QwPysg7A/edit?gid=69736821#gid=69736821&fvid=998460810).
2.   Above the table, click the "Views" button and select the "Group by Status & Sort by Last Updated (Most Recent First)" view.
3.   Go to the themes with Status: P2 Needs Testing.
4.   Select a theme to message and write your WordPress username in the notes column so everyone else knows you're working on it.
5.   Click the link in the "Latest Trac Ticket" column to go to Trac.
6.   Post a comment for the developer on the Trac ticket, using the "If the theme has not been tested" message template below.
7.   Check the box in the "Message posted for theme dev" column.
8.   Move on to another theme.

## Template Messages

### If the theme has been tested:

```markdown
Hi @USERNAME,

Recently, the Accessibility Team [https://make.wordpress.org/accessibility/2026/05/06/accessibility-ready-requirements-updated/ updated the accessibility-ready tag requirements.]

All accessibility-ready themes must update their themes to meet the new standards if they would like to keep using the `accessibility-ready` tag. Many of the requirements are essentially the same, but there are some new requirements. [https://make.wordpress.org/themes/handbook/review/accessibility/required/ Read the updated requirements.]

Theme authors have until **June 30th, 2026** to begin the progress to update their themes — either to fix the accessibility or to remove the tag.

I conducted an initial accessibility-ready review of your theme. The following items are among the issues that need to be addressed but are not a complete list:

* ISSUE 1
* ISSUE 2
* ISSUE 3
* Missing new requirement: `accessibility.txt` file.

You can find a more thorough [GOOGLE-SHEETS-LINK accessibility audit of your theme here]. Note: I did not complete the testing due to reaching a maximum number of issues.

If you would like to keep using the accessibility-ready tag, please read the updated guidelines thoroughly, update your theme, and request a new review when you're ready. [https://make.wordpress.org/accessibility/request-an-accessibility-ready-review/ Request an accessibility review here.]

If you don't want to keep using the tag or cannot improve your theme's accessibility, please remove the tag from your theme before June 30th.

Thank you!
```

### If the theme has not been tested:
Ideally, this message is only used for the P2 themes.

```markdown

Hi @USERNAME,

Recently the Accessibility Team [https://make.wordpress.org/accessibility/2026/05/06/accessibility-ready-requirements-updated/ updated the accessibility-ready tag requirements.]

All accessibility-ready themes must update their themes to meet the new standards if they would like to keep using the `accessibility-ready` tag. Many of the requirements are essentially the same, but there are some new requirements, so all developers will need to update their theme. [https://make.wordpress.org/themes/handbook/review/accessibility/required/ Read the updated requirements.]

Theme authors have until **June 30th, 2026** to update their themes — either to fix the accessibility or to remove the tag.

If you would like to keep using the accessibility-ready tag, please read the updated guidelines thoroughly, update your theme, and request a new review when you're ready. [https://make.wordpress.org/accessibility/request-an-accessibility-ready-review/ Request an accessibility review here.]

If you don't want to keep using the tag or cannot improve your theme's accessibility, please remove the tag from your theme before June 30th.

Thank you!

```
