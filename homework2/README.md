# Ted talks dataset

## Data source
This dataset contains MOST VIEWED TED TALKS so far scraped for the website.

Starting page: https://www.ted.com/talks?page=1&sort=popular

## Data fileds
* `speakers` - String, e.g.`'Ken Robinson'`
* `views` - list, e.g.` ['7.3M','7.2M','7M','6.9M']`
* `time.sleep` - int, e.g.`5`


## Data volumes
20 pages in the sort of most viewed(720talks)

## License
CC 4.0

## Notes
* When there are some errors, check from the first step, especially check if your urls work.
  in my case, the second url is wrong, so the next page repeat the data of first url.
* Use `time.sleep` to anti-scrape when requests are mass, e.g. over than 10 pages.
* Use `utf_8_sig` in the csv to keep the data in the right format.
* Use `extend` if you set the first page data in a list, not `append`, which is used for String.
