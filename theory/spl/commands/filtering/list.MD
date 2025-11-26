# LIST 

The command "LIST" is used in the context of Splunk AppInspect, which is a tool used to inspect and validate the quality of Splunk apps and add-ons. The "LIST" command in Splunk AppInspect is used to list various types of items such as groups, checks, and tags. For example, you can use the command "splunk-appinspect list groups checks tags" to list all groups, checks, and tags.

The command is also used with various options, such as "--included-tags" and "--excluded-tags", to filter the results. For instance, you can use the command "splunk-appinspect list checks --included-tags splunk-appinspect" to list only the checks that are tagged with the "splunk-appinspect" tag.

Some of the available options for the "LIST" command include:

groups: lists all groups
checks: lists all checks
tags: lists all tags
version: displays the version of Splunk AppInspect
custom-checks-dir: specifies a custom directory for custom checks
The "LIST" command is typically used with the following syntax: "splunk-appinspect list [OPTIONS] LIST_TYPE..." where LIST_TYPE can be any combination of "groups", "checks", or "tags".
