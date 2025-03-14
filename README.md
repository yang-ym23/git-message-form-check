# Git Message Testing Tool

This is a simple web-based **Regular Expression Testing Tool** that allows users to test predefined regex patterns against input text. It provides immediate feedback on whether the input matches the selected regex pattern.

## Features

- **Predefined Regular Expressions**
  - Commit message format validation
  - Merge message format validation
  - Branch name format validation
- **Custom Input Testing**
- **Case-Insensitive Matching Option**
- **User-Friendly Interface**
- **Real-Time Feedback on Matching Results**

## Technologies Used

- **HTML** (Structure)
- **CSS** (Styling)
- **JavaScript** (Logic and Functionality)

## How to Use

Click [here](https://yang-ym23.github.io/git-message-form-check/) to use the tool.

## Regular Expressions Used

### 1. Commit Message Format
```
^(add|chore|docs|feat|fix|other|perf|refactor|res|revert|style|test)(\([\w\-]+\))?:\s.{1,100}(\n\n.{1,1000})?(\n\n(Closes|Fixes|Resolves)\s#\d+)?$
```
Validates commit messages following conventional commit standards.

### 2. Merge Message Format
```
^merge (branch '[\w\-/]+' into '[\w\-/]+'|pull request #\d+ from '[\w\-/]+')$
```
Validates merge commit messages.

### 3. Branch Name Format
```
^(master|dev|(feat|fix)/[\w\-_]+)$
```
Validates branch names based on naming conventions.
