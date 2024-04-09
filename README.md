# MyVSCode

My VSCode

## What to do in a fresh computer

- Download and Install VSCode
  - installer or extract: all good
  - try the latest
- Install extenstions
  - Theme
  - Markdown
  - Dev (Java, Python, Go ...)
  - Docker, Kubernetes
  - GitHub
  - ...
- Theme
- Settings
  - Auto Save
  - Format on file save
  - Opt out the data collection
  - Change default terminal from PowerShell to be Command Prompt

## RegEx replace

```text
I use VSCode to update my md file.

there are some bullet points like these:
1. title 1
2. title 2
3. title 3
4. title 4

How to quickly update them to 

## Step 1: title 1
## Step 2: title 2
## Step 3: title 3
## Step 4: title 4
```

In Visual Studio Code, you can use regular expressions with the find and replace feature to quickly update your Markdown file. Here's how you can do it:

1. Press `Ctrl + H` (Windows/Linux) or `Cmd + Shift + H` (Mac) to open the Replace widget.
2. Check the box with `.*` on the left side of the input box. This enables regular expression mode.
3. In the "Find" input box, type: `(\d+)\. (.*)`
4. In the "Replace" input box, type: `## Step $1: $2`
5. Click on "Replace All" to replace all occurrences.

This regular expression captures the number and the title separately, and then in the replacement, it formats them according to your desired format.

Make sure to double-check your file after replacing to ensure everything looks correct.
