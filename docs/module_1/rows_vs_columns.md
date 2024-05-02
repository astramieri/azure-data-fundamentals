# Row-Store vs Column-Store

When looking at tabular data there are two ways data can be stored:
- **row-store**
    - data is organized in rows
    - good for general purpose databases
    - suited for OLTP
    - great when needing all possibile columns in a row is important
    - not the best at anlytics or massive amounts of data
- **column-store**
    - data is organzied into columns
    - faster at aggregating values for analytics
    - great for vast amount of data
    - suited for OLAP
    - greater when you only need a few columns