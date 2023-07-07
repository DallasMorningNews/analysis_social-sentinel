# Social Sentinel
Analysis code for investigative series on Social Sentinel.

## How we reported the Social Sentinel stories
In public, the social media monitoring service Social Sentinel said its tool was not designed to surveil students. In conversations with schools,  the company promoted its ability to “mitigate” and “forestall” protests. It also allowed schools to enter keywords related to events that could become contentious and wrote a white paper about how it could monitor demonstrations. 

Colleges across the country used the features. One school, Kennesaw State University, surveilled a town hall protest. Another college,  UNC-Chapel Hill, tracked student demonstrations against a campus Confederate statue and protests against a school’s handling of a cheerleader’s rape allegation.
Our reporting found at least 38 colleges used the tool, including to monitor student protests. We analyzed thousands of innocuous tweets flagged by the service and found a former college football player who spent months in jail after campus police were alerted to his posts and a former company employee who described the technology as “snake oil.” 
Social Sentinel said its AI technology could help schools prevent suicides and shootings. Our investigation found no evidence that any student lives were saved because of an alert from the service. A dozen school officials raised concerns about the system, with some estimating its false positive rate at close to 99%. Legal and privacy experts said its use was troubling.

After _The Dallas Morning News_ published the  first story, a North Carolina legislator launched an inquiry into school use of surveillance technology and UNC ended its contract with Social Sentinel. The story received attention from local, state and national media organizations. At least 15 college newspapers wrote about our story, and it was even taught in university courses.

Our project was a comprehensive examination of the use of social media surveillance software on college campuses. We hope more journalists  — particularly student journalists — will continue to examine the impact of artificial intelligence.

## Hypothesis and data collection
After discovering that UNC had used Social Sentinel during protests against a racist statue on campus, I suspected other schools were using the tool to monitor campus demonstrations. After three years and dozens of open records requests, my Berkeley classmate and colleague Derêka Bennett and I obtained more than 56,000 pages of documents that showed other schools were using the tool.  

To compile a list of schools that used Social Sentinel, we obtained data from GovSpend, a database of government spending. We also reviewed student news stories and other public records. Nearly all of the schools in our database came from references in other schools' documents. Our database included only those schools that were mentioned at least twice. We also confirmed use of the service with university officials. Once we suspected a school had used the service, we filed records requests at that college. 

We added information about schools’ student populations to the database using data from univstats.com and used Google Maps to find the location of a central administrative building on campus. This data was then put into DataWrapper to build the map you see in both stories. 

In all, we analyzed nearly 4,200 posts flagged by the service. Those were either included in the emails we obtained from schools themselves or through links to PDFs inside of the documents. 

## Methodology
To analyze the PDF alerts, we first had to convert all of the document images into machine-readable text using an optical character recognition tool. Then we wrote a Python script to parse the documents. We noticed that the format of the data changed over time, which required us to modify our script to accommodate these differences. After parsing all of the documents into a single spreadsheet, we used a machine learning tool called a tokenizer to make lists of every word in each post, removed punctuation and common words and then counted the number of times a word appeared in the posts. These results were visualized in a bar chart, which ran inside the second story. 

We stored our documents in Google Drive, Google Pinpoint and DocumentCloud. Dereka and I read each one and took notes on their contents.  We used those to create memos that helped us write a footnoted findings memo. 

## Overcoming challenges
We faced delays in getting the records we requested, astronomical cost estimates for information — one school quoted us $40,000 — and university lawyers who objected to providing the material. Some schools said there were no records responsive to our request when it was clear there were. Several schools failed to provide the alerts from the service even though they were included in the scope of every records request we filed. We also faced hurdles with universities that gave us  non-machine readable PDF files, which did not allow us to click links to obtain more information. 

We resolved some problems by working with public records officers to craft requests that allowed us to access the information we needed in a more timely, less expensive manner. 

## Bulletproofing the story
We followed a standard fact-checking process starting with a 33-page memo of every notable finding from all of our sources of material. Each finding was footnoted and hyperlinked. When referencing information in documents we included the name of the document, the page number it was found on and the relevant passage. 


These findings were a culmination of the reporting we did in the 2021-2022 school year and were presented as part of an investigative seminar led by multi-Pulitzer Prize winning journalist and head of UC Berkley’s Investigative Reporting Program David Barstow. Throughout the reporting process we met with Barstow and _The Dallas Morning News’_ investigations editor Karisa King.

Our findings memo served as the spine of the project and allowed us to spend less time footnoting the drafts. Each story went through several rounds of revisions from the investigations editor, managing editor and executive editor of _The News_. The story text and reporting material were also reviewed by _The News’_ attorney.

If you haven’t already, we’d encourage you to read our stories at _The Dallas Morning News_ here: https://interactives.dallasnews.com/2022/social-sentinel/

https://interactives.dallasnews.com/2022/the-black-box-social-sentinel/.

The text of the stories is also available without a paywall on the Pulitzer Center website. 

_Arijit (Ari) D. Sen is an AI Accountability Fellow at the Pulitzer Center and a Computational Journalist at The Dallas Morning News._