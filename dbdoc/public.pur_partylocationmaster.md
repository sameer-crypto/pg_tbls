# public.pur_partylocationmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| locationid | integer | nextval('pur_partylocationmaster_locationid_seq'::regclass) | false |  |  |  |
| headid | integer |  | true |  |  |  |
| locationname | varchar(250) |  | true |  |  |  |
| locationcode | varchar(250) |  | true |  |  |  |
| ischild | boolean | false | true |  |  |  |
| locationtype | integer |  | true |  |  |  |
| isauthorized | boolean |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp(6) without time zone |  | true |  |  |  |
| inactivedate | timestamp(6) without time zone |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| stateid | integer |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pur_partylocationmaster_pkey | PRIMARY KEY | PRIMARY KEY (locationid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pur_partylocationmaster_pkey | CREATE UNIQUE INDEX pur_partylocationmaster_pkey ON public.pur_partylocationmaster USING btree (locationid) |

## Relations

![er](public.pur_partylocationmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
