# nosql-challenge
Challenge 12


# Change the data type from String to Integer for RatingValue

establishments.update_many(
    {'RatingValue': {'$regex': '[1-6]'}},
    [{'$set': {'RatingValue': {'$toInt': '$RatingValue'}}}]
    )
    
OR

establishments.update_many(
    {'RatingValue':{'$in': ["1", "2", "3", "4", "5"]}},
    [{'$set':{'RatingValue':{'$toInt':'$RatingValue'}}}]
    )
