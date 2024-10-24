# public.hr_employeeprevdecl

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| employeedeclid | integer | nextval('hr_employeeprevdecl_employeedeclid_seq'::regclass) | false |  |  |  |
| employeeid | integer |  | false |  |  |  |
| isactive | boolean | false | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| short_name | varchar(100) |  | true |  |  |  |
| description | varchar(1000) |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| fromdate | date |  | true |  |  |  |
| todate | date |  | true |  |  |  |
| prevempsal | numeric(18,2) |  | true |  |  |  |
| prevemptds | numeric(18,2) |  | true |  |  |  |
| prevempproftax | numeric(18,2) |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| hr_employeeprevdecl_pkey | PRIMARY KEY | PRIMARY KEY (employeedeclid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| hr_employeeprevdecl_pkey | CREATE UNIQUE INDEX hr_employeeprevdecl_pkey ON public.hr_employeeprevdecl USING btree (employeedeclid) |

## Relations

![er](public.hr_employeeprevdecl.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
