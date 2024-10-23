# public.pm_parametermaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| parameterid | integer | nextval('pm_parametermaster_parameterid_seq'::regclass) | false |  |  |  |
| parametercode | varchar(100) |  | true |  |  |  |
| parameterdescription | varchar(255) |  | true |  |  |  |
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
| iscancelled | boolean | false | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| Unique_parametercode | UNIQUE | UNIQUE (parametercode) |
| pm_parametermaster_pkey | PRIMARY KEY | PRIMARY KEY (parameterid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| Unique_parametercode | CREATE UNIQUE INDEX "Unique_parametercode" ON public.pm_parametermaster USING btree (parametercode) |
| pm_parametermaster_pkey | CREATE UNIQUE INDEX pm_parametermaster_pkey ON public.pm_parametermaster USING btree (parameterid) |

## Relations

![er](public.pm_parametermaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)