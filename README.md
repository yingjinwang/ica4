# ica4
USF projects for the SQL questins
## Description of datasets.yingjin.yelp_reviews


## Question #1
1.	How many restaurants with stars?

```sql
SELECT stars, count(business_name) as number_restaurants
FROM yingjin.yelp_reviews 
WHERE stars <> '?'
group BY 1
ORDER BY stars
```

![ica4](ica4/1.png)

## Question #2
2.	How many check-ins during Monday to Friday?

```sql
SELECT weekday, count(checkins) as number_checkins
FROM datasets.yelp_checkin
group BY 1
ORDER BY weekday
```

![ica4](ica4/ica4/2.png)
