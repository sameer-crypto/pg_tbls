# public.pay_leavestructuremaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| leave_structure_id | integer | nextval('pay_leavestructuremaster_leave_structure_id_seq'::regclass) | false |  |  |  |
| leave_structure_name | varchar |  | true |  |  |  |
| fromdate | date |  | true |  |  |  |
| isactive | boolean |  | true |  |  |  |
| isauthorized | boolean |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| isdefault | boolean | false | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| leavestructurename_uq | UNIQUE | UNIQUE (leave_structure_name) |
| pay_leavestructuremaster_pkey | PRIMARY KEY | PRIMARY KEY (leave_structure_id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| leavestructurename_uq | CREATE UNIQUE INDEX leavestructurename_uq ON public.pay_leavestructuremaster USING btree (leave_structure_name) |
| pay_leavestructuremaster_pkey | CREATE UNIQUE INDEX pay_leavestructuremaster_pkey ON public.pay_leavestructuremaster USING btree (leave_structure_id) |

## Relations

![er](public.pay_leavestructuremaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
