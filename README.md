Summary of the free Mixpanel course: https://mixpanel.com/content/guide-to-product-analytics/report/

# Chapter 1: introduction

/

# Chapter 2: Measure value: The foundations of product analytics

## How does my product bring value

User needs to find value in your product while using it, if not, they will stop using it.

examples

- make life cheaper
- make life easier
- make life more convenient
- ...

Important to know when the user experiences the value from you product.

## How can I monetize my product

- Transactional

  - 1 time fixed price
  - eg. Komoot 1 time purchase of a region

- Subscription

  - Users pay a fixed price per unit of time
  - eg. Netflix - 10 euro for an unlimited amout of movies

- Licensing

  - Users pay a license fee to use, sell, or copy a product.
  - eg. Mapbox - monthlee fee to develop to use the software.

- Freemium
  - part free, part paid
  - eg. Spotify

Non monetaire ways of getting back value

- User's attention

  - advertising
  - eg. YouTube

- User's data
  - gathering date to learn patterns about users
  - eg. Google

_Insights_

Important to understand the user and it's willingness to pay.
This can differ in different segments of users.

Willingess to pay can very over time. Certing external or macro economical factors can impact the user's willingbess to pay

- eg. covid
- eg. high gass prices
- ...

### Measuring product value

Hard to measure how the users perceived that value of your application, this is often "Fuzy". We need to make this more measureable by making some assumptions.

- eg. How much fun and entertainment users are getting from a video streaming service

  - how much videos does a user watch a day/week/month
  - how long does the user wactch videos

In some cases, the assumptions are too risky and qualitative feedback will be needed on top of the quantitative feedback gathered by Analytics tools. When combine both of these researches we can jump to conclusions.

- eg. Anxiety reduction in users of a meditation

  - questions

    - (quantitative) completion rate of meditation sessions
    - (quantitative) weekly retention of users
    - (qualitative) What is your perceived anxiety

  - Conclusions
    - How does using the app on a weekly basic impact the user's anxiety.
    - How does completing x percentage of sessions impact the user's anxiety
      ...

- eg. Rodi

  - questions

    - (quantitative) How many rides are completed on Rodi per week
    - (qualitative) How many rides does the user do in totals (with and without Rodi)

  - Conclusions
    - How much does the user depend on Rodi for his bike rides.

## What is a value moment

Your product’s value moment is an event, an action, or a series of events and actions that represent the moment that a user found value in your product

Tinder -> like on a photo
MyFitnessPall -> completion of a workout
Twitch -> watch +5 minutes of a stream
DocuSign -> Sign a contract
Rodi -> Start a ride

_setup moments_

Moments that a user needs to perform before they can come to the value moment

Setup moments should be kept as low as possible as user's might dropof before experiencing the value moment.

examples

- creating an account
- adding a credit card
- extensive onboarding
- notification permissions
- adding friends

## Which metrics should i pick to measure product success.

[TODO] mixpanel course on defining north start metrics -> https://mixpanel.com/content/guide-to-product-metrics/full-report/

Value moments are building blocks to good product adoption. The more value moments, the more oportunities to build a habit for the user.

_North Star metric or Focus metric_

Turning value into a single key metric

- Tinder -> get a match
- Therapy app -> # of user who complete a - session weekly
- MyFitnessPall -> # of user who complete a workout weekly
- DocuSign -> # of contracts signs monthly
- DocuSign -> Time between sharing and signing
- Rodi -> # of rides over 1km completed - weekly

## Where do product leaders typically go wrong when defining their value metric?

north start metric should

- is responsive to product changes
- is an aggregate measure of the product’s value for its users
- can be readily tied to value for the business or to broader company goals
- is expected to remain relevant for a reasonable duration of time

A north start metric should be accompanied with a set of metrics that might impact the north start metric and help understand any changes in this north start metric.

# Chapter 3: Get to know your users

## What’s user segmentation in product analytics?

User segmentation => dividing users in groups/ cohorts based on a user property (country, gender).

In Mixpanel every event is linked to a user. You can create segments/ cohorts based on every event or datapoint you have on a user

Based on events

- users who is vs users who isn't logged in
- users who went through the onboarding vs users who skipped the onboarding

Based on properties

- users in Europe vs users in America
- users that are male vs users that are female

## What’s DAU/ WAU/ MAU?

DAU -> Daily active users

WAU -> Weekly active users

MAU -> Monthly active users

### Defining active usage

Don't define active as "opens the app".

An active user is a users who finds value in your product

- x amount of time in app
- x amount of actions taken
- executed a specific action
  - eg. AirBnb: clicked on at least one property
  - eg. Facebook: liked or commented on at least on post
  - ...

## When should I measure DAU/WAU/MAU?

### ✅ DAU/WAU/MAU as one of the ways to assess overall business health

**Other relevant metrics**

Churn

- Customer churn refers to the natural business cycle of losing and acquiring customers. Every company — no matter the quality of its products or customer service — experiences churn. Generally speaking, the less churn you have, the more customers you keep.

LTV

- Customer lifetime value (CLV, or CLTV) is a metric that indicates the total revenue a business can reasonably expect from a single customer account throughout the business relationship.

ARR/ MRR

- annual recurring revenue/ montly recurring revenue

All these metrics, alongside DAU/WAU/MAU give a good overall indicator of the health of your company/ product. It is important that have a clear and strict definition of Active. If not DAU/WAU/MAU will become a vanity metric.

Vanity Metric

- Vanity metrics are statistics that look spectacular on the surface but don't necessarily translate to any meaningful business results.

As discussed above, these statistics can give some insights on the health of a company, but their importance should not be overstated. They don't give all the insights in the product.

### ✅ DAU/WAU/MAU to track seasonal changes for your business

DAU/WAU/MAU can be used to detect seasonal changes of your business.

- A cycling app will most likely have more users in the summer and less in the winter.

### ✅ DAU/WAU/MAU to measure marketing funnel effectiveness

Keeping an eye out on the DAU during marketing campaigns can help you with figuring out what marketing strategy works.

Looking at the churn of these users is really important here. It is more valuable to have 10 users from a campaign that continue to use the app than 100 users that only open the app once.

### ❌ DAU/WAU/MAU for product benchmarking

It is hard to compare Active users troughout apps for severall reasons

1. Companies define "Active" differently
2. Different industries need different benchmarking

### ❌ DAU/WAU/MAU for building better products

DAU/WAU/MAU can be a health indicator of your product. But growing DAU can be caused by different factors than the quality of your product

- Marketing (budget)
- Exposure
- Seasonal changes
- ...
