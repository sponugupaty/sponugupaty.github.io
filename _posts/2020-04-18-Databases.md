# Databases And SQL 

Here's the table of contents:

1. TOC
{:toc}

## Introduction

> SQL is an easy language to learn and difficult to master 

Inspired by Josh Kaufman's talk [here](https://www.youtube.com/watch?v=5MgBikgcWnY) , I wanted to run an experiment of spending about 20 hours in reading up about Databases & SQL and being useful with these skills . I also find that lots of people assume that they know SQL well , but are unable to have a fruitfu conversation after the initial handwaving .This article is an effort to fix that by pointing to some very good resources around the web and books which can help us in deep diving into this area.

This article is broadly split into Applied SQL - quickly being useful in querying a dataset using a database of your choice AND Investigatng how commercial database engines work under the hood . 

## Applied SQL - Introduction ( 2 Hours )

    Section useful to get a quick start 

One of the best resources I found on the web to quickly get started with learning the basics of SQL was 
[here](https://www.selectstarsql.com/) . This cool utility is created and  maintained by a Stripe engineer using client side SQL which means that you dont need to download and configure any software . You can edit and run queries on the browser itself . Each of the questions has the authors solutions to compare against .The choice of dataset is intriguing but gothic in nature - death row inmates executed in state of texas since 1976 .

Cheatsheet of contents  :

- Uses the SQLLite syntax instead of SQL Server . For example - use of LIMIT instead of TOP in select statements
- SELECT can be followed by special character * ( when we want all the columns ) or column names  
- Block Comments and single line commenting possible 
- FROM clause comes always after the SELECT . Is needed only when selecting from a table 
- By default carries out integer division . Multiply by 1.0 for floating point division
- Always a good idea to figure out if the version of SQL engine you are using is case sensitive
- WHERE clause allows us to filter rows that meet certain criteria
- Can use arithmetic operators ( < , <= , > etc ) to build clauses
- LIKE is the most powerful string operator . LIKE with % ( pattern matching ) and _ ( single character) is useful
- Aggregation funtions take multiple rows of data and turn them into one number
- COUNT most used aggregate function and COUNT(<<col_name>>) returns count of non-null rows 
- NULL is the value of an empty entry . Is not same as '' empty string or 0
- COUNT( * ) gives us the number of rows with alteast one of their columns is not null 
- CASE WHEN acts as a big if statement 
- AVG , LEN , MIN , MAX are the other aggregate functions of interest 
- GROUP BY helps us to split the data set and apply aggregate functions within each group
- HAVING is a post aggregation filter ( similar to WHERE clause )
- INNER JOIN ( JOIN by default) drops unmatched rows 
- LEFT JOIN preserves the rows of the left table 
- RIGHT JOIN preserves the rows of the right table 
- OUTER JOIN preserves the rows in both the tables 
- SELF JOIN powerful way of letting rows get information from other parts of the table 
- Nested queries will need some practice and understanding of use cases

---

## Applied SQL - Level Up ( 2 Hours )

```SQL
use computer

--Ex1 - Find the model number, speed and hard drive capacity for all the PCs with prices below $500. Result set: model, speed, hd.
select model , speed , hd
from PC (nolock)
where price < 500

--Ex2 - Find printer makers. Result set: maker.
select b.maker
from Printer a (nolock)
join Product b (nolock)
on a.model = b.model

--Ex 3 - Find the model number, RAM and screen size of the laptops with prices over $1000.
select model , ram , screen 
from Laptop (nolock)
where price > 1000

--Ex 5 - Find the model number, speed and hard drive capacity of the PCs having 12x CD and prices less than $600 or having 24x CD and prices less than $600.
select model , speed , hd 
from PC ( nolock )
where  cd in ('12x', '24x' )
and price < 600 

--Ex 6 - For each maker producing laptops with a hard drive capacity of 10 Gb or higher, find the speed of such laptops. Result set: maker, speed.
select b.maker , a.speed 
from laptop a (nolock)  
join product b (nolock ) 
on a.model = b.model 
where a.hd >= 10

--Ex 7 - Find out the models and prices for all the products (of any type) produced by maker B
-- find out the types of products maker B makes 
--select * from product where maker = 'B'
select a.model , b.price
from product a (nolock)
join
( 
select model , price from PC 
union 
select model , price from laptop
)b 
on a.model = b.model
where a.maker = 'B'


--Ex 8 - Find out the makers that sale PCs but not laptops.
-- Interesting !!
select distinct a.maker 
from product a (nolock)
where a.type = 'PC'
and a.maker not in 
( select maker
	from product (nolock)
	where type = 'Laptop'
	)

-- Ex 10 - Find the printers having the highest price. Result set: model, price.
-- Interesting!!
select model , price 
from printer
where price = ( select max(price) from printer)

-- Ex 11 - Find out the average speed of PCs.
--select * from PC
select avg(speed) from PC

-- Ex 71 - Find all the makers who have all their models of PC type in the PC table
--select * from PC


--Ex 13 Find out the average speed of the PCs produced by maker A.
select avg(a.speed) 
from PC(nolock) a 
join product (nolock) b 
on a.model = b.model 
where b.maker = 'a'

--Exercise 3
```




## Lists

Here's a list:

- item 1
- item 2

And a numbered list:

1. item 1
1. item 2

## Boxes and stuff

> This is a quotation

{% include alert.html text="You can include alert boxes" %}

...and...

{% include info.html text="You can include info boxes" %}

## Images

![](/images/logo.png "fast.ai's logo")

## Code

General preformatted text:

    # Do a thing
    do_thing()

Python code and output:

```python
# Prints '2'
print(1+1)
```

    2

## Tables

| Column 1 | Column 2 |
|-|-|
| A thing | Another thing |

## Footnotes

[^1]: This is the footnote.

