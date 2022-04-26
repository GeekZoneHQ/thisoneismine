# This One Is Mine
> This is my issue. There are many like it, but this one is mine.

## What it does
A super simple GitHub action that allows anyone to assign themselves to an issue by using the `/mine` command in a comment.

## Why?

FOSS projects want to empower people to contribute to their projects, without waiting for permission. This is at odds with the fact that GitHub does not natively provide a way for people to assign themselves to an issue unless they are already an org member, so this action fills that gap.

## How it works
On new issue comment,
- If comment does not contain `/mine`, do nothing.
- If issue assignee is not None, do nothing.
- Else, assign the user who created the comment to the issue.


## Recommended accompaniments

Use in conjunction with our [Weeping Angel](https://github.com/GeekZoneHQ/weepingangel) action to ensure that only issues which are actively being worked on remain assigned.
