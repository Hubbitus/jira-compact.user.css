# jira-compact.user.css
Css styles to compact jira (>=6.1) representation (now support up to version 8.1). For example to use with Stylish Chromium and Firefox extension

Any feedback welcome!

## How to use
For Chrome/Chromium browswers I use it in nice [Stylish](https://chrome.google.com/webstore/detail/stylish/fjnbnpbmkenffdnngjfgmeleoegfcffe?hl=ru) extension.
I have not tested, but should work in [Firefox Stylish](https://addons.mozilla.org/ru/firefox/addon/stylish/) variant too (please let me known if it is not true).

You may install it from Stylish site: https://userstyles.org/styles/112544/jira-6-1-compact-theme in that case updates will be propogated automatically.

Alternatively: Just click button "Create style" and copy/paste content of file https://raw.githubusercontent.com/Hubbitus/jira-compact.user.css/master/jira-compact.user.css.

## What it is

I use Jira in my day job. It very good famous and extensible bug tracker. But even I use wide monitor additionally to notebook their design seems to me very sprawling.

That style was born several month when I tried there and there reduce elements and spaces between, move description right, highlight title and key fields like status…

As it style 100 words have worth less than example looks (for simplicity and easy distinguishing I will show screenshots of original Jira in Firefox and in Chromium with that style applied)


### Screenshots

1) Jira 3 column dashboard (aaa layout):
![Original jira 3 column dashboard](screenshots/Dashboard-aaa-Original.png)
![Compacted jira 3 column dashboard](screenshots/Dashboard-aaa-Compact.png)

Please note - **even more rows and columns in widgets tables - scrolling dissapeared**.

2) Jira 2 column dashboard (ba layout):
![Original jira 2 column (second wide) dashboard](screenshots/Dashboard-ba-Original.png)
![Compacted jira 2 column (second wide) dashboard](screenshots/Dashboard-ba-Compact.png)

*Unfortunately there one implementation details quirk: Widgets at right must be at colors 5 (blue - #003366), 6(violet - #3C78B5) or 7 (grey - #bbbbbb). Otherwise you may just change style*.

3) Issues and its list (search, filter).
![List of issues original look](screenshots/List-of-issues-Original.png)
![List of issues compact view](screenshots/List-of-issues-Compact.png)

You may see several enhancments here:
* Issue details from center moved to right. So, you start read from problem, meta information also at top right.
* Left list do not truncate issue summary at half of word - instead multiline used.
* If you use [Threaded comments plugin](https://marketplace.atlassian.com/plugins/com.atlassian.jira.threadedcomments.threaded-comments) there are also few changes - compactnesss, highlight odd lines and fir like/dislike bug appearence as a bonus.
![threaded comments](screenshots/Comments-thread.png)

## Licensing
Work distributed under terms of [CC BY - Creative Commons Attribution](http://creativecommons.org/licenses/by/4.0/)

## Changelog
2019-11-15 Fix issues list in Epic: Fix width of status and percentage column.
2019-11-05 Add styling of "Two dimensional filter statistic" gadget
2019-05-08 Styling dashboards left list and widgets spacing. Do not indent <p> in dashboards. Support Jira 8.1.
2019-03-11 Fix epic linked tasks table glitch
2019-02-03 Fix status labels break on epic issues list
2018-12-22 Show linked issues full list always with scrolling in blocks
2018-11-01 Do not wrap assignee in epic tasks list
2018-01-26 Change applying regexp for all domains starting from "jira."
2018-01-19 Firefox compatability fix for gadgets

- Drop line-height: 1.4em; for p::first-letter
- For gadgets table allign header by center and all cells by middle vertically.
2017-10-18 Allow break long task statuses by full words like "Selected for development"
2017-06-14 Add support of custom text-fields in issue
2017-03-04 Fix main task description edit with issue
2017-02-27 Decrease labels padding for dashboards, smaller issue-list action button, fix issues sub-list line doubling due to the icons
2017-02-17 Fix scrolling and tune some other styles like icons in issues search left navigation list
2017-02-17 Compact also Epic issues list in issue
2017-02-17 Fix height of buttons and menus on issue like "edit", "comment", "assign"…
2017-02-09 Issues sub-list correct percentage column style
2017-02-01 Fix linked issues sub-list always full
2017-01-24 Compact dates in dashboards widgets
2017-01-16 Fix row ordering arrows in one line in sub-tasks list. Compact (v) sign on completed sub-tasks
2016-07-26 Show linked issues full list
2016-07-21 Compact style also pie-chart on dashboard
2016-07-12 Fix issue with time spent/remaining bars in sub-tasks
2016-07-12 In sub-tasks task list arrows for reordering place in one line to decrease height
2016-07-11 Allow wrap labels in td
2016-07-04 Update to fresh Jira styling of dashboards.
2016-06-02 Format editable fields and icons
2016-05-31 Fix sub-tasks list and editing area.
2016-04-15 Fix line height (introduced by previous font size change). Add terms (code, kbd, tt) highlight.
2016-04-14 Change main font to slightly large (x-small -> small) to normal distinguish bold. Fix editable for Jira version 6.4.11