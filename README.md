# web-scrapper
This project simulates scraping data from multiple web pages in parallel. It showcases the benefits of parallelism for I/O-bound tasks.

## Functionality:
Users provide a seed URL and a maximum depth for crawling.
The program crawls websites in parallel, following links and extracting data.
Scraped data is stored in a structured format (e.g., database, text file).
Users can see crawled URLs and extracted data.

## Sequential Crawling:
Implement a baseline function that crawls websites one after another, following links and scraping data.
This highlights the inefficiency of waiting for each page to be downloaded before continuing.
## Parallel Crawling:
Use a process pool or asynchronous framework to crawl websites in parallel.
Distribute website URLs from a queue to processes or coroutines for independent crawling.
Employ synchronization mechanisms (e.g., queues) to manage the crawling queue and avoid duplicate visits.
This approach utilizes multiple processes or event loops to download pages simultaneously, significantly improving performance.

## Showcasing Parallelism:
Measure the execution time of crawling sequentially and in parallel with different numbers of processes/coroutines.
Analyze the impact of available network bandwidth and disk speed on performance gains.
Discuss the trade-offs between parallelism (process/coroutine creation overhead) and network/disk limitations in this context.
