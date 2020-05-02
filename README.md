# Ms Fox
This is an `Amazon Product Scraper` built using `scapy` module of `python`

# Features
it scrape various things
- Product Title
- Product Image
- Product Price
- Product Rating
- Product Description
- Product Reviews
- Product Brand
- Product Colour
(for educational purpose)

By default it scrapes `Mobile Phones` of `5 Pages` from `Amazon`.
In case you want to change it to scrape other product, follow the instructions
1. Open file `/amazon_scraper/spiders/amazon_scraper.py`
2. Change the `urls` list at line `16`
3. Update `no_of_pages` variable to change number of pages to be scraped

# Execute Amazon Scraper
there are two ways to execute scraper
### First one
you can directly execute `run.sh` file using shell
```sh
sh ./run.sh
```

### Second one
you can execute the following command
```bash
scrapy crawl amazon_scraper -o ./data/data.json
```

It will create `data.json` file inside the `data` folder containing all the scraped data in `JSON` format and all the images will be saved in `data/img/full` folder.

# Sample Data
Already fetched sample data is available in `data` folder

# Troubleshooting
If `data.json` file doesn't generate in proper format then just delete `data.json` file and `img` folder.  
Now you good to go ;)

# Preresuisites
- you have to install `scrapy`
- you have to install `pillow`

## Error
Due to COVID19 there is no display of price of products on amazon and also amazon changes some css style for the site that's why it will not scraping some products and not working fine.
Wait for the update



Created with :heart: by Rishabh Sharma
