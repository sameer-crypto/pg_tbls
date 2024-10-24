# public.pm_maintenancescheduledetails

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| detailid | integer | nextval('pm_maintenancescheduledetails_detailid_seq'::regclass) | false |  |  |  |
| scheduleid | integer |  | false |  |  |  |
| fromdate | timestamp without time zone |  | true |  |  |  |
| todate | timestamp without time zone |  | true |  |  |  |
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
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pm_maintenancescheduledetails_pkey | PRIMARY KEY | PRIMARY KEY (detailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pm_maintenancescheduledetails_pkey | CREATE UNIQUE INDEX pm_maintenancescheduledetails_pkey ON public.pm_maintenancescheduledetails USING btree (detailid) |

## Relations

![er](public.pm_maintenancescheduledetails.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
