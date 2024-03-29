# Houston Meetup Data

For this month's [data jam](https://www.meetup.com/Houston-Data-Visualization-Meetup/events/233079777/), we will be working with Meetup data from the Houston area.  This data is sourced from Meetup's API.

We have the data available in **csv**, each in their respective directories.

## Data

The data are found in the following files:

1. **groups.csv**: groups.csv -- Unique entry for every group

  | Column    | Description                                |
  |----------:|--------------------------------------------|
  | id     | unique group id|
  | name | group name|
  | urlname    | url to meetup page|
  | rating     | average rating for meetup events |
  | created | date of creation |
  | description    | meetup description |
  | organizerName      | organizer's name |
  | organiserMemberID | organizer's unique member ID |

1. **members.csv**: members.csv -- One entry for every member-group pair

  | Column | Description                                |
  | ------:| ------------------------------------------ |
  | id   | unique member id |
  | name  | group name |
  | joined  | date member joined the group [in milliseconds from epoch](https://currentmillis.com/)|
  | topics  | topics of interest set by member |
  | groupId  | unique group id (matches group ids in `groups.csv`)                            |

1. **venues.csv**: Each row contains the schedule and type of the primary election by state and party

  | Column | Description                                |
  | ------:| ------------------------------------------ |
  | id   | unique venue id |
  | name  | venue id |
  | city  | city venue is located in |
  | address_1   | address line 1 for venue |
  | address_2  | address line 2 for venue |
  | lat   | latitude                              |
  | lon   | longitude                              |


## Sources
- [micahstubbs/modeling-worked-example](https://github.com/micahstubbs/modeling-worked-example)
- [Neo4j example](https://github.com/neo4j-meetups/modeling-worked-example)
- [Meetup's API](https://www.meetup.com/meetup_api/)
