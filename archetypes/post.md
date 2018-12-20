---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
publishDate: "{{ .Date.Format "2006-02-01" }}"
archives: "{{ dateFormat "2006" now }}"
tags: []
---
