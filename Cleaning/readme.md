<p align="center">
  <a href="https://us.pg.com/" target="_blank">
    <img width="150" src="https://upload.wikimedia.org/wikipedia/fr/thumb/d/d3/Procter_%26_Gamble_2013_%28logo%29.png/1920px-Procter_%26_Gamble_2013_%28logo%29.png" alt="logo">
  </a>
</p>

<h2 align="center">Cleaning up the data</h2>

---

In order to more efficiently use our data, we started by cleaning up the dataset.

## 💡 Idea

In order to get better data, and better results on our testing, we decided to consider both the training and the testing dataset when we were calculating averages as well as minimums an maximums.

After doing this process, we noticed a considerable accuracy boost.

## 🌐 Adding features with the second dataset

The more relevant features we have, the better it is, that is why we have used the data set "consumeractions" which gives relevant information about the engagement rate of each user toward the brands of P&G, and the level of interest of these users. We used this data set to add new features to our user's rows :
'interested_by_fairypeps_email' : says if a user has had actions related to an email about FAIRY PEPS
'level_of_interest_about_marketing' : a continuous value between 0-1 depending on whether the user has just opened an email or has gone further by clicking or using coupons.
'number_of_actions' : counter of the actions of the user related to emails, coupons or search bar of the website

## 📚 Description

|            column name            | data type |                                                        description                                                        | nan fill |
| :-------------------------------: | :-------: | :-----------------------------------------------------------------------------------------------------------------------: | :------: |
|              userId               |  String   |                                              A unique string for every user                                               |          |
|                age                |   Float   |                 A float describing the user age, with `0.0` being the youngest user and `1.0` the oldest                  | Average  |
|              gender               |   Float   |                          A float describing the user's gender. `1.0` for women and `0.0` for men                          |          |
|            scentLover             |   Float   |           A float describing the user's interest for ecology ranging between `0.0`: none, to `1.0`: passionate            | Average  |
|            ecoInterest            |   Float   |            A float describing the user's interest for scents ranging between `0.0`: none, to `1.0`: passionate            | Average  |
|             MrPropre              |   Float   |                               Has the user used `MrPropre` ? `1.0` he has, `0.0` he hasn't                                |  `0.0`   |
|              Antikal              |   Float   |                                Has the user used `Antikal` ? `1.0` he has, `0.0` he hasn't                                |  `0.0`   |
|               Ariel               |   Float   |                                 Has the user used `Ariel` ? `1.0` he has, `0.0` he hasn't                                 |  `0.0`   |
|               Dash                |   Float   |                                 Has the user used `Dash` ? `1.0` he has, `0.0` he hasn't                                  |  `0.0`   |
|               pods                |   Float   |                                 Does the user use `pods` detergent ? `1.0` yes, `0.0` no                                  |  `0.0`   |
|              powder               |   Float   |                                Does the user use `powder` detergent ? `1.0` yes, `0.0` no                                 |  `0.0`   |
|              liquid               |   Float   |                                Does the user use `liquid` detergent ? `1.0` yes, `0.0` no                                 |  `0.0`   |
|        electricToothbrush         |   Float   |                              Does the user use an electric toothbrush ? `1.0` yes, `0.0` no                               |  `0.0`   |
|             likesPets             |   Float   |           A float describing the user's interest for pets going between `0.0`: hates them, to `1.0`: loves them           | Average  |
|              hasPet               |   Float   |                                       Does the user have pets ? `1.0` yes, `0.0` no                                       |  `0.0`   |
|         daysSinceActivity         |   Float   | A float describing the number of days since last activity, with `0.0` being the latest activity date and `1.0` the oldest | Average  |
|            nbChildren             |   Float   |           A float describing the number of children of a user, with `0.0` being none and `1.0` being 5 or more            | Average  |
|              magasin              |   Float   |                            Is the shop closest to the user a `Magasin` ? `1.0`: yes, `0.0`: no                            |  `0.0`   |
|          moyenneSurface           |   Float   |                        Is the shop closest to the user a `moyenneSurface` ? `1.0`: yes, `0.0`: no                         |  `0.0`   |
|            superMarket            |   Float   |                          Is the shop closest to the user a `superMarket` ? `1.0`: yes, `0.0`: no                          |  `0.0`   |
|            hyperMarket            |   Float   |                          Is the shop closest to the user a `hyperMarket` ? `1.0`: yes, `0.0`: no                          |  `0.0`   |
|               drive               |   Float   |                             Is the shop closest to the user a `drive` ? `1.0`: yes, `0.0`: no                             |  `0.0`   |
|           hardDiscount            |   Float   |                         Is the shop closest to the user a `Hard Discount` ? `1.0`: yes, `0.0`: no                         |  `0.0`   |
|   interested_by_fairypeps_email   |   Float   |                        Has the user had an action related to the brand "FAIRY PEPS" ? `1.0`: yes, `0.0`: no               | `0.0`  |
| level_of_interest_about_marketing |   Float   |                        A float describing the user's level of interest about P&G marketing ranging between `0.0`: email opened, to `1.0`: coupon used                                                    | Average  |                                               
|         number_of_actions         |   Float   |                        counter of the actions of the user related to emails, coupons or search bar of the website                                                                                                   | Average  |
|            washDishes             |   Float   |                        Has the user a washDishes ? `1.0`: yes, `0.0`: no                                                                                                   |    `0.0`      |
