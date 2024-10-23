# public.hr_esirulesmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| esirulesid | integer | nextval('hr_esirulesmaster_esirulesid_seq'::regclass) | false |  |  |  |
| applicablefrom | timestamp without time zone |  | true |  |  |  |
| applicableto | timestamp without time zone |  | true |  |  |  |
| companyesi1 | numeric(18,2) |  | true |  |  |  |
| companyesi2 | numeric(18,2) |  | true |  |  |  |
| employeeesi1 | numeric(18,2) |  | true |  |  |  |
| employeeesi2 | numeric(18,2) |  | true |  |  |  |
| amount | numeric(18,2) |  | true |  |  |  |
| roundofftype | integer |  | true |  |  |  |
| isactive | boolean | false | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| esirules_pkey | PRIMARY KEY | PRIMARY KEY (esirulesid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| esirules_pkey | CREATE UNIQUE INDEX esirules_pkey ON public.hr_esirulesmaster USING btree (esirulesid) |

## Relations

![er](public.hr_esirulesmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)