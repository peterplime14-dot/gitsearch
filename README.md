# 🔎 gitsearch.sh

A CLI tool for searching GitHub repositories and users using parallel requests and Python-based JSON parsing.

## ✨ Features

Search GitHub repositories or users via the GitHub API
Optional programming language filtering
Configurable number of results
Fast parallel fetching
Lightweight and dependency-friendly

## ⚙️ Requirements

· bash 

· curl

· python3

· git (optional, for cloning repositories)

Core utilities: sed, tail, wc, cut

## 📦 Installation

Download the script:

git clone https://github.com/peterplime14-dot/gitsearch
 
· cd repo-directory

· chmod +x gitsearch

· gitsearch

Option 2

· chmod +x gitsearch

· mv gitsearch ~/.local/bin/

## 🚀 Usage

./gitsearch.sh [FLAGS] [search_term] [language]


## 🎛️ Flags

· -u, --user → search for users instead of repositories

· -n, --num → number of results to display (default: 15)

## 🧠 Behavior

First non-flag argument is treated as the search query
Second non-flag argument is used as the language filter
Multi-word queries are automatically URL-encoded
Results are fetched from the GitHub API and parsed using Python

## 💡 Examples

 ./gitsearch.sh machine learning python

· Search repositories about machine learning in Python.

 ./gitsearch.sh -u john

· Search for GitHub users named “john”.

 ./gitsearch.sh -n 10 "data structures" cpp
 
· Show 10 C++ repositories about data structures.
