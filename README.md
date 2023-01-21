# WhatsApp-Messages-DB-Analysis-Using-SQL
## Introduction
This repository contains a collection of SQL code snippets for analyzing WhatsApp chat backups stored in an SQLite database. The code utilizes `sqlite3` to query the data and `pandas` to return results in a tabular format. The code samples demonstrate how to retrieve statistics on various aspects of WhatsApp conversations such as:

* Media sent: Count of different media types (image, audio, sticker, document, video, gif)
* Voice records: Audio duration
* Textual analysis: Most common messages, emojis used per chat
* Emojis and reactions: Reaction distribution, reactions vs chats, starred messages
* Fun facts: Top chats, first ever chat, longest messages, longest daily chatting streaks
* Chat statistics: Number of messages sent by each sender in a specific chat, media distribution, media vs chat, total messages per chat, sender wise messages per chat, highest daily message for one chat over time, timeline of highest number of messages sent in one chat for each month, highest number of messages sent in one day for each chat, and count of times a chat had the highest daily messages.

The output of each query is a DataFrame that can be used for further data analysis and visualization. The provided queries can help you to get deeper insights into your WhatsApp chats. The code uses various SQL techniques such as subqueries, correlated subqueries, joins, window functions, text and date manipulation functions to efficiently analyze the data.

## DataSource
WhatsApp chat backup data in the form of an SQLite database. The data is sourced and extracted from personal WhatsApp chats, For more details [See](https://www.group-ib.com/blog/whatsapp-forensic-artifacts/), The database contains 153 tables, and the code in this repository utilizes a subset of them for the analysis.<br>

Tables Snapshot : 

![Tables](https://github.com/abdulrahmankhayal/WhatsApp-Messages-DB-Analysis-Using-SQL/blob/main/Tables_SnapShot.png)
