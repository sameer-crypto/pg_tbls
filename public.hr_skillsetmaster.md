# public.hr_skillsetmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| skillsetid | bigint | nextval('hr_skillsetmaster_skillsetid_seq'::regclass) | false |  |  |  |
| skillsetcode | varchar |  | false |  |  |  |
| skillsetname | varchar |  | false |  |  |  |
| remarks | varchar |  | true |  |  |  |
| isactive | boolean |  | true |  |  |  |
| inactivedate | date |  | true |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| hr_skillsetmaster_pkey | PRIMARY KEY | PRIMARY KEY (skillsetid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| hr_skillsetmaster_pkey | CREATE UNIQUE INDEX hr_skillsetmaster_pkey ON public.hr_skillsetmaster USING btree (skillsetid) |
| uq_skillsetcode | CREATE UNIQUE INDEX uq_skillsetcode ON public.hr_skillsetmaster USING btree (lower((skillsetcode)::text)) |
| uq_skillsetname | CREATE UNIQUE INDEX uq_skillsetname ON public.hr_skillsetmaster USING btree (lower((skillsetname)::text)) |

## Relations

![er](public.hr_skillsetmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)