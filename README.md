# Web_scrapper
This Python script is designed to crawl through a website starting from a given URL and extract useful contact information such as email addresses and phone numbers. Additionally, it searches for specific keywords like "contact", "email", "phone", and "about" throughout the entire website to help identify relevant content sections. It uses a combination of requests for HTTP requests, BeautifulSoup for parsing HTML, and regular expressions to match email and phone number patterns. The script is particularly useful for quickly analyzing a site’s publicly visible contact information.

When executed, the script begins by crawling the main page and follows all internal links recursively, ensuring that it only navigates within the same domain. On each page it visits, it extracts the raw HTML content and uses pattern matching to detect and collect email addresses and phone numbers. To ensure relevance, it filters out numbers that are too short or too long, effectively excluding irrelevant data like tracking IDs or postal codes. It supports various phone number formats, including standard Indian mobile numbers (+91-xxxxxxxxxx, 080-xxxxxxx, 99999 99999) and common landline formats. Duplicates are automatically removed from the final output, and only unique emails and phone numbers are printed.

In addition to data extraction, the script also performs a keyword search by rendering each page and checking for the presence of user-defined keywords in the visible text. If a keyword is found, it is reported in the console, giving insight into which pages contain relevant content areas.

### Below is a sample output of the script:

![image](https://github.com/user-attachments/assets/e90e366d-4429-4328-96a8-0a5aaa1dc344)


This script is particularly helpful for developers, testers, and digital researchers who need to extract contact information from websites efficiently. 

### ❗ Warning & Disclaimer ❗
⚠️ FOR TESTING PURPOSES ONLY ⚠️
- This script is intended strictly for educational or testing use only.
- Do NOT use this script to scrape or crawl websites without permission.
- The developer is not responsible for any misuse, legal issues, or damages caused by running this code.
