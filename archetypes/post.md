---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
publishDate: "{{ dateFormat "2006-02-01" now }}"
archives: "{{ dateFormat "2006" now }}"
tags: []
---
