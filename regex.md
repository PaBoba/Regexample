# Regex Tutorial
The purpose of this tutorial is to break down a regex example and explain what each part of the regex does. Today, we will examine a regex for identifying file names that have the common image extensions PNG, JPG, and JPEG. PNG is a lossless image file type, whereas JPG and JPEG are lossy.

# Table of Contents
[The Regex](#the-regex)\
[Regex Start](#regex-start)\
[File Name](#file-name)\
[File Format Start](#file-format-start)\
[File Format](#file-format)\
[Regex End](#regex-end)

# The Regex
```
^.+\.(png|PNG|jpg|JPG|jpeg|JPEG)$
```

# Regex Start
```
^
```
The caret symbol is an anchor point that denotes the start of the match. 

# File Name
```
.+
```
The period is a wildcard character, meaning it can match any character. Since any valid character can be in the file name, we us the wildcard character. The plus is a quantifier that says there must be at least one character. So combined, this means the file name can consist of any character of length at least one.

# File Format Start
```
\.
```
File formats are separated with a period. In regex, we need to escape the period with a backslash because the period would be a wildcard otherwise.

# File Format
```
(png|PNG|jpg|JPG|jpeg|JPEG)
```
The | character is an or operator that means any of these strings can match. Here we've listed the file formats we want to match in both upper and lower cases. 

# Regex End
```
$
```
The dollar symbol is an anchor point that denotes the end of the match. 

# About the Author
Randy Wu is a coding bootcamp student and UX designer.\
His Github: https://github.com/PaBoba
