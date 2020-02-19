# NoteLog Data Feed Service ![Test Status](https://github.com/NoteLog/notelog-data/workflows/Test/badge.svg)

A cron service that feeds data from various places into NoteLog's main database for later use.

## Sources

Current data sources implemented includes:

### GitHub

Using the Google's [GitHub API Go library](https://github.com/google/go-github), it retrieves the combined list of my personal repositories and those that I starred.

### Blog

Scrapes my website [posts page](https://tansawit.me/posts) for the list of posts. It then visits each of those posts, extracting the relevant information (title, description, categories, tags, url)
