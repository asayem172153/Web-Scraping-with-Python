# Web Scraping with Python
Here, I have done some basic web scraping 
***Working Steps:***  
1. First task is to collect/extract data from a website. Here, I use https://kathika.org/stories to extract data. From HTML data I have to collect **Book Name, Author Name, Content (Story)**. But the challenges is **Book Name** is present into the first page But **Author Name, Content** of each book is different and have to collect from different pages.
2. To overcome the Challenges for each book we have to render the link to open the book into a another page. Then again **GET** the response from those pages where we collect **Author Name and Content (Story)** of the book. Then Marge them into a dictionary like that {Book Name : [Author][Content]}
3. After that save the file into a **JSON** file. Used **JSON** file becuase it's useful to store nested or structured type data.
4. Here comes the part of Data Cleaning to maintain the integrity of the book content. For easy to use First we load the **JSON** data. Then, check whether there is any **HTML** content contain into the book content or not. After checking, remove unnecessary expressions using **RegEx**.
5. Display Writers number of book written
6. Save each books as **txt** file. Where file name is **book_name.txt**. inside that file is **book_content**.
7. Save each **book_name** and **writer_name** in **csv** file.
