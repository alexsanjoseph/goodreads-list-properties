# Goodreads - List Properties Database

This script takes the link of a list from the Goodreads and scrapes through each of the pages and find the following properties:

- book_name
- author
- rating
- votes
- description
- book_type - Paperback, Hardback, etc.
- no_of_pages
- first_published - Date at which the book was published first, if available.
- isbn13
- genre - The most common tag for the book

It works as of `2017/02/25` but can't guarantee if it will work in the future :D.

Currently it is configured to work in the Best Books List
he `Pool` parameter. But I didn't want to give a large number and DOS the system

# Datasets

## Most Popular Books Dataset

I've also included the results of running the script on the Best Books List (which is the largest list in Goodreads AFAIK).
`https://www.goodreads.com/list/show/1.Best_Books_Ever`

It has the details of 47610 books.


# Known Bugs

- If there is no description for a book, sometimes the first comment is displayed instead of the description.
- The script fails for a random reasons for a a very small number of cases, but I haven't spent the time to go and debug the issue since it affect <1% of the cases, and none of the more interesting books (Top 100 pages or so)

Scraping is inherently susceptible to bugs so please suggest in Issues if there is something else wrong.
