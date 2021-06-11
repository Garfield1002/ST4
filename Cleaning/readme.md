# Cleaning up the Data

## 📚 Description

|            column name            | data type |                                                        description                                                        | nan fill |
| :-------------------------------: | :-------: | :-----------------------------------------------------------------------------------------------------------------------: | :------: |
|              userId               |  String   |                                                                                                                           |          |
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
|   interested_by_fairypeps_email   |   Float   |                                                                                                                           | Average  |
| level_of_interest_about_marketing |   Float   |                                                                                                                           | Average  |
|         number_of_actions         |   Float   |                                                                                                                           | Average  |
|            washDishes             |   Float   |                                                                                                                           |          |
