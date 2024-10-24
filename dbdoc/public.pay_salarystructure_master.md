# public.pay_salarystructure_master

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| salstructureid | integer | nextval('pay_salarystructure_master_salstructureid_seq'::regclass) | false |  |  |  |
| salarystructure | varchar |  | true |  |  |  |
| gradeid | integer |  | true |  |  |  |
| applicable_from | timestamp(6) without time zone |  | true |  |  |  |
| applicable_to | timestamp(6) without time zone |  | true |  |  |  |
| isauthorized | boolean |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| isactive | boolean | false | true |  |  |  |
| short_name | varchar |  | true |  |  |  |
| ctc | numeric |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pay_salarystructure_master_pkey | PRIMARY KEY | PRIMARY KEY (salstructureid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pay_salarystructure_master_pkey | CREATE UNIQUE INDEX pay_salarystructure_master_pkey ON public.pay_salarystructure_master USING btree (salstructureid) |

## Relations

![er](public.pay_salarystructure_master.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
