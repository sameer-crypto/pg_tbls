# public.pm_breakdowncomplaintlogdetails

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| complaintdetailid | integer | nextval('pm_breakdowncomplaintlogdetails_complaintdetailid_seq'::regclass) | false |  |  |  |
| complaintid | integer |  | false |  |  |  |
| assetid | integer |  | false |  |  |  |
| natureoffaultid | integer |  | false |  |  |  |
| breakdownreasonid | integer |  | false |  |  |  |
| expecteddate | timestamp without time zone |  | true |  |  |  |
| remarks | varchar(255) |  | true |  |  |  |
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
| complaint | text |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pm_breakdowncomplaintlogdetails_pkey | PRIMARY KEY | PRIMARY KEY (complaintdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pm_breakdowncomplaintlogdetails_pkey | CREATE UNIQUE INDEX pm_breakdowncomplaintlogdetails_pkey ON public.pm_breakdowncomplaintlogdetails USING btree (complaintdetailid) |

## Relations

![er](public.pm_breakdowncomplaintlogdetails.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
