---
layout: default
title: Using CLI
nav_order: 2
has_children: true
permalink: /docs/using-cli
---

# CLI Example
`src_dir_path` = input =  -i
<br>
`dst_dir_path` = output = -o

## Case 1. `src_dir_path` = `dst_dir_path`
### 1.1. Directory(Folder)
If your input is a directory path and `src_dir_path` = `dst_dir_path`, Here.
>
#### 1.1.1. 
```bash
# Only input without output
$ incoming -i "~/ic_demo/input_path"
```
or
```bash
# If you set "src_dir_path" == "dst_dir_path" on `ic_settings.json`
$ incoming
```
Result
```
~/ic_demo
    /input_path
    /input_path-ic
```
- $ic will make directory in `src_dir_path`'s parent.
- set name {prefix} + {`src_dir_path`'s name} + {suffix}. 
- The suffinx named '-ic' is setted by default. You can change in `ic_settings.json`
>
#### 1.1.2.
```bash
$ incoming -i "~/ic_demo/input_path" -o "~/ic_demo/input_path"
```
Go to 1.1.1.
>
#### 1.1.3.
```bash
~/ic_demo/input_path/ $ incoming -o "~/ic_demo/output_path"
```

>
### 1.2. Single File
You can also convert single file.
>
#### 1.2.1. 
```bash
# single files
```

## Case #2. Source path ≠ Destination path



# Command line reference

To make it as easy as possible to write documentation in plain Markdown, most UI components are styled using default Markdown elements with few additional CSS classes needed.
{: .fs-6 .fw-300 }

The following details all the available options in the command line interface. This information may be accessed at any time by running `incoming --help`. Please run this command on your own system as available options may vary depending on operating system and system hardware.

For reference, the following was generated by the Windows version of incoming. Options may vary slightly depending on hardware / operating system. Run `incoming --help` for valid options for your system.