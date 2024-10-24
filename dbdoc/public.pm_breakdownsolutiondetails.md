# public.pm_breakdownsolutiondetails

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| detailid | integer | nextval('pm_breakdownsolutiondetails_detailid_seq'::regclass) | false |  |  |  |
| solutionid | integer |  | false |  |  |  |
| complaintdetailid | integer |  | false |  |  |  |
| isbreakdownreason | boolean | false | false |  |  |  |
| employeeid | integer |  | false |  |  |  |
| fromtime | timestamp without time zone |  | true |  |  |  |
| totime | timestamp without time zone |  | true |  |  |  |
| remarks | varchar(255) |  | true |  |  |  |
| status | varchar(50) |  | true |  |  |  |
| isspareconsume | boolean | false | false |  |  |  |
| sno | integer |  | false |  |  |  |
| isactive | boolean | false | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pm_breakdownsolutiondetails_pkey | PRIMARY KEY | PRIMARY KEY (detailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pm_breakdownsolutiondetails_pkey | CREATE UNIQUE INDEX pm_breakdownsolutiondetails_pkey ON public.pm_breakdownsolutiondetails USING btree (detailid) |

## Relations

![er](public.pm_breakdownsolutiondetails.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
