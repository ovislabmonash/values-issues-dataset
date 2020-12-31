# Dataset from a Case Study of Human Values in Issue Discussions

## Description

This is a dataset from our journal paper titled: "_*Human Values in Software Development Artefacts: A Case Study on Issue Discussions in Three Android Applications*_". This paper is submitted to the Information and Software Technology Journal: Special Issue on Value and Waste in Software Engineering. 

## Directory Information

All files are saved using csv format with `|` as the separator.

- `proposed-values.csv`: list of proposed values
	
	- `id`: identifier of the value
	- `value_name`: name of the value

- `issues.csv`: list of issues

	- `issue_id`: identifier of the issue
	- `title`: the title of the issue
	- `project_name`: the project name of the issue
	- `artefact_url`: the url to the actual issue in GitHub

- `issue-posts.csv`: list of posts associated with issues

	- `post_id`: identifier of the post
	- `issue_id`: identifier in which issue the post belongs to
	- `body_text`: the post in a text format
	- `body_html`: the post in HTML format
	- `created_at`: the date the post was created
	- `type`: type of the post, either `title` of the issue or `post` of the issue

- `values-label.csv`: the values label of the issue

	- `issue_id`: identifier of the issue (see `issues.csv`)
	- `post_id`: identifier of the post (see `issue-posts.csv`)
	- `proposed_values_id`: identifier of the proposed value (see `proposed-values.csv`)