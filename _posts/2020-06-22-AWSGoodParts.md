# AWS - Good Parts

Here's the table of contents:

1. TOC
{:toc}

## Basics
- Chasing the best tool for the job is insidious trap at the beginning of the project
- This is **optimization Fallacy** and is in the same category as premature optimisation
- Searching for the optimal solution is almost always expensive 
- If we believe we can discover the best option by testing each option , then we are delusional
- Instead use a **Deafult Heuristic**
- The premise of this heuristic is that when the cost of acquiring new information is high and the consequence of deviating
  from a default choice is low, sticking with the default will likely be the optimal choice 
- A default choice is any option that gives you very high confidence that it will work. Most of the time, it is something you’ve used
  before. Something you understand well. Something that has proven itself to be a reliable way for getting things done in the space you’re   operating in.
- Your default choice doesn’t have to be the theoretical best choice. It doesn’t have to be the most efficient. Or the latest and greatest.   Your default choice simply needs to be a reliable option to get you to your ultimate desirable outcome. Your default choice should be       very unlikely to fail you; you have to be confident that it’s a very safe bet. In fact, that’s the only requirement.

## DynamoDB 
- Although Amazon calls , DynamoDB as database , it can be seen as a durable B-tree dadatastructure in the cloud
- Its is more similar to Redis than MySQL , but unlike Redis is immediately highly durable and consistent 
- It can replace a relationship database , provided you can get away with using a B-tree 
- DynamoDB requires that you do most of the querying in your application code 
- You can read a single value or contiguos range of values 
- But the sorting , filtering , or aggregation needs to happen in the application code 
- **Query processing on the app side is not just incovinient but has performance implication as well** 
- Relational DB run the queries closer to the data and send the results over the wire 
- **This is a major downside of DynamoDB**
- **Cost of storage , is another factor . Almost 10 times the cost of S3 storage**
- **Request Pricing** is also another key factor . On-demand $1.25 per million writes and $0.25 for million reads
- start with on-demand pricing( no capacity mgmt burden)  and then consider to provisioned capacity( cost savings )


