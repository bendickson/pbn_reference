## IMPORT A `USER`
------
> A `USER` = A MEMBER (AND/OR SPEAKERS, ASSOCIATION ADMINS, AND MORE TBD)

_the `USER` object can also have custom fields added to the below_

| Login         | Firstname       | Lastname        | Email                     |
| ------------- |:----------------|-----------------| --------------------------|
| `dummy_login` |`dummy_firstname`| `dummy_lastname`| `dummy_email@mydomain.com`|

## IMPORT A `COURSE`
------
> A `COURSE` = AN INDIVIDUAL SESSION AND HOLDS INFO ABOUT THE SESSION ATTRIBUTES (*NAME*, CODE, CATEGORY, PRICE, ACTIVE, DESCRIPTION, CATALOG, ...)

_the `COURSE` object can also have custom fields added to the below_

| Name               | Code     | Description           | Category   | Price    |
| ------------------ |:---------|:--------------------- |:-----------|:---------|
| *European History* | *HIST01* | *An intro course...*  |**Custom**  |**Custom**|
| `PBN Session Name`      | `4650-10`| `This program will...`|`2016 Conference`| `$25` |

## IMPORT A `GROUP`
------
> A `GROUP` = TBD

| Group               | Description   | Key
| ------------------ |:---------|:--------------------- |
| *New employees* | *All new employees should be members of this group* | *An intro course...*  | xyzhna
|  `?`| `?`| `?`

## IMPORT A `BRANCH`
------
> A `BRANCH` = A PBN CUSTOMER (EACH BRANCH CAN HAVE IT'S OWN UNIQUE BRANDING, CONTENT, ETC. BUT STILL TESTING)

| Branch             | Description  |
| ------------------ |:------------|
| *sales* | *All sales people belong to this branch* | 
|  `nala`| `All USERS for customer nala`| 

## IMPORT A **CATEGORY**
------
>`CATEGORIES` = PACKAGES AND BUT THIS NEEDS TO BE THOUGHT OUT B/C YOU CAN SELL AN ENTIRE CATEGORY AND NALA HAS SUB-CATEGORIES OR CHILD CATEGORIES IN TALENTLMS ARCHIECTURE (MAYBE THERE IS A DIFFERENT WAY TBD)

_Cat level 1 > Cat level 2 > Cat level 3_

| Category (Parent)   | Category (Child)  | Category (Child)
| ------------------ |:---------|:--------------------- |
| *Cat level 1* | *Cat level 2* | *Cat level 3*  | 
|  `2016 Conference`| `Ethics`| `Legal`

## ENROLL A `USER` TO A `COURSE`
------
> `USER` TO A `COURSE` = TBD

| Usertocourses               | Course + (Code)
| ------------------ |:---------|
| *dummy_login* | *European History (HIST01)* |
|  `?`| `?`| `?`

## ADD A `USER` TO A `GROUP`
------
> `USER` TO A `GROUP` = TBD

| Usertocourses               | Group
| ------------------ |:---------|
| *dummy_login* | *New employees* |
|  `?`| `?`| 

## ADD A `USER` TO A `BRANCH`
------
> `USER` TO A `BRANCH` = A USERNAME TO A PBN CUSTOMER

| Usertobranches        | Branch
| ------------------ |:---------|
| *dummy_login* | *sales* |
|  `username`| `nala`| 


## ADD A `COURSE` TO A `GROUP`
------
Coursetogroups; group

> `COURSE` TO A `BRANCH` = A SESSION TO A PBN CUSTOMER

| Coursetogroups (Course + (Code))    | Group
| ------------------ |:---------|
| *European History (HIST01)* | *New employees* |
|  `PBN Session Name (4650-10)`| `?`| 

## ADD A **COURSE** TO A **BRANCH**
------
Coursetobranches; branch

> `USER` TO A `BRANCH` = A USERNAME TO A PBN CUSTOMER

| Coursetobranches  (Course + (Code)  | Branch
| ------------------ |:---------|
| *European History (HIST01)* | *sales* |
|  `PBN Session Name (4650-10)` | `nala`| 