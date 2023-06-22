Summary of the free Mixpanel course: https://mixpanel.com/content/guide-to-product-analytics/report/

- [Chapter 1: introduction](#chapter-1-introduction)
- [Chapter 2: Measure value: The foundations of product analytics](#chapter-2-measure-value-the-foundations-of-product-analytics)
  - [How does my product bring value](#how-does-my-product-bring-value)
  - [How can I monetize my product](#how-can-i-monetize-my-product)
  - [What is a value moment](#what-is-a-value-moment)
  - [Which metrics should i pick to measure product success.](#which-metrics-should-i-pick-to-measure-product-success)
  - [Where do product leaders typically go wrong when defining their value metric?](#where-do-product-leaders-typically-go-wrong-when-defining-their-value-metric)
- [Chapter 3: Get to know your users](#chapter-3-get-to-know-your-users)
  - [What’s user segmentation in product analytics?](#whats-user-segmentation-in-product-analytics)
  - [What’s DAU/ WAU/ MAU?](#whats-dau-wau-mau)
  - [When should I measure DAU/WAU/MAU?](#when-should-i-measure-dauwaumau)
- [Chapter 4: Analyze user engagement](#chapter-4-analyze-user-engagement)
  - [What is my product usage interval?](#what-is-my-product-usage-interval)
  - [Who are my power/core/casual users?](#who-are-my-powercorecasual-users)
  - [What is the right definition of power/core/casual users for my product](#what-is-the-right-definition-of-powercorecasual-users-for-my-product)
  - [How can I tie active usage to my value exchange (monetization) model?](#how-can-i-tie-active-usage-to-my-value-exchange-monetization-model)
  - [Besides segmenting by level of engagement, how else can you analyze different groups of users with product analytics?](#besides-segmenting-by-level-of-engagement-how-else-can-you-analyze-different-groups-of-users-with-product-analytics)
- [Chapter 5: retain your users](#chapter-5-retain-your-users)
  - [Where are my users dropping off?](#where-are-my-users-dropping-off)
  - [Should B2B and B2C companies measure drop off on their user’s path to value differently?](#should-b2b-and-b2c-companies-measure-drop-off-on-their-users-path-to-value-differently)
  - [How can I measure user drop off?](#how-can-i-measure-user-drop-off)
  - [Why should I measure retention?](#why-should-i-measure-retention)
  - [How do I measure retention?](#how-do-i-measure-retention)
- [Chapter 6: Grow and scale](#chapter-6-grow-and-scale)
  - [How do you measure growth?](#how-do-you-measure-growth)
  - [how should your growth strategy change as you company matures?](#how-should-your-growth-strategy-change-as-you-company-matures)
  - [How can a product manager drive growth?](#how-can-a-product-manager-drive-growth)
  - [Where are my most valuable users coming from?](#where-are-my-most-valuable-users-coming-from)

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
  - eg. Netflix - 10 euro for an unlimited amount of movies

- Licensing

  - Users pay a license fee to use, sell, or copy a product.
  - eg. Mapbox - monthly fee to develop to use the software.

- Freemium
  - part free, part paid
  - eg. Spotify

Non monetary ways of getting back value

- User's attention

  - advertising
  - eg. YouTube

- User's data
  - gathering data to learn patterns about users
  - eg. Google

_Insights_

Important to understand the user and it's willingness to pay.
This can differ in different segments of users.

Willingness to pay can very over time. Certain external or macro economical factors can impact the user's Willingness to pay

- eg. covid
- eg. high gas prices
- ...

### Measuring product value

Hard to measure how the users perceived that value of your application, this is often "Fuzzy". We need to make this more measurable by making some assumptions.

- eg. How much fun and entertainment users are getting from a video streaming service

  - how much videos does a user watch a day/week/month
  - how long does the user watches videos

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

Setup moments should be kept as low as possible as user's might drop-off before experiencing the value moment.

examples

- creating an account
- adding a credit card
- extensive onboarding
- notification permissions
- adding friends

## Which metrics should i pick to measure product success.

[TODO] mixpanel course on defining north start metrics -> https://mixpanel.com/content/guide-to-product-metrics/full-report/

Value moments are building blocks to good product adoption. The more value moments, the more opportunities to build a habit for the user.

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

- annual recurring revenue/ monthly recurring revenue

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

It is hard to compare Active users throughout apps for several reasons

1. Companies define "Active" differently
2. Different industries need different benchmarking

### ❌ DAU/WAU/MAU for building better products

DAU/WAU/MAU can be a health indicator of your product. But growing DAU can be caused by different factors than the quality of your product

- Marketing (budget)
- Exposure
- Seasonal changes
- ...

# Chapter 4: Analyze user engagement

## What is my product usage interval?

There is no interval of desired usage intervals for every app. It highly depends on the industry the app is in.

| Industry     | Examples             | Interval         | Value moment                            | Context                                                                |
| ------------ | -------------------- | ---------------- | --------------------------------------- | ---------------------------------------------------------------------- |
| Contact      | Gmail, Slack, Teams  | Hourly           | Refreshing/ answering a message         | Expected to use these tools on a constant base throughout the day      |
| Social Media | Facebook, TikTok     | Daily            | Viewing and interacting with a post     | To create a habit in this scene, frequent user engagement is necessary |
| Health       | Allan, MCC           | Monthly - weekly | Booking a Doctor via the app.           | The user does not need to use the app frequently to find it valuable   |
| Sport        | Rodi, Komoot, Strava | Weekly           | Logging a sport session through the app | Logging a sport activity daily is physically difficult.                |

## Who are my power/core/casual users?

Determine what event is your "AHA moment", and see what type of users are in the top

- 10% -> power user
- 20% - 50% -> core users
- 50% - 90% -> casual users
- (below - one time users)

## What is the right definition of power/core/casual users for my product

### Frequency

How often does a user return to the product compared to the medium.

### Breadth

Does a user use all the more advanced features or just the main/ core option/ feature

### Depth

How many times has the user experienced a value moment.

## How can I tie active usage to my value exchange (monetization) model?

The type of users you have will have impact on the preferred monetization model for your product.

- Frequency: daily -> adds make sense as the users spend a lot of time on your platform.
- Frequency: monthly -> monthly/ yearly subscriptions make sense.

## Besides segmenting by level of engagement, how else can you analyze different groups of users with product analytics?

- percentiles of activity (to identify power users)
- free vs paid users
- new vs existing users
- operating system
- region
- monthly vs yearly subscribers

# Chapter 5: retain your users

## Where are my users dropping off?

> "Users are more likely to retain when they successfully experience value in your product early and often."

### Big drop-off points

1. Registration/ onboarding

There should be a minimum amount of steps before the user get's to the value of the app. If there is a cumbersome registration flow or a lengthy onboarding, the user might drop off before even using the app.

2. The value moment

The promised value of the application is not what the user expected.

3. The value exchange

The value exchange moment is where you ask something from your user (monetization)

## Should B2B and B2C companies measure drop off on their user’s path to value differently?

No, the users of the applications are still regular people who decide if the subscriptions should be renewed. Drop off should be measured the same.

## How can I measure user drop off?

### Setup Funnels

The most important funnel to keep track of is the one from **first time opening the app** towards the **first value moment**.

Now we can detect where we can improve our user drop off.

## Why should I measure retention?

> “Does my product bring value to users–over and over and over again?”

Low churn and high retention rate are two sides of the same coin—and reliable signals of lasting product success.

### mistakes when defining retention metrics.

**Focus on revenue**

The monthly revenue of a SaaS company is not an indicator of retention. You can loose a lot of users but gain even more because of marketing efforts. this is not sustainable.

**Choosing the wrong frequency**

More info in the "What is my product usage interval?" section above.

**Failure to tie retention back to value**
Your retention metric should reflect the number of retained users who experience value.

## How do I measure retention?

N Day retention

- calculates the percentage of users who come back on a specific day.

Unbounded retention

- calculates the percentage of users who come back on a specific day (or week, month, etc.) or any time unit afterwards.

# Chapter 6: Grow and scale

## How do you measure growth?

Growth is difficult to measure

- eg. Amount of user -> can be misleading because of marketing efforts/budgets.

**Determine a north start metric that indicates growth**

## how should your growth strategy change as you company matures?

Measuring growth is even more important when your target audience moves from a niche audience to a more brought audience.

In the early days you will try a lot of different things to look for PMF (product market fit) later, with the gained insides from earlier, more specific iterations will be made.

## How can a product manager drive growth?

Find what actions lead to value moments

- eg. Facebook - a person needs 7 - 10 friends to not immediately churn

> The strategy is to try and understand, as soon as possible, what a retained user regularly does and then try to get users who are not retained to form the same habits.

## Where are my most valuable users coming from?

By Using Mixpanel Segments you can attach a segment where the user found the product. We can later see what marketing efforts lead to the most users that didn't churn.
