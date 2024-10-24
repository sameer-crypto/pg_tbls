# public.pay_employee_entitlement_master

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| entitlementid | integer | nextval('pay_employee_entitlement_master_entitlementid_seq'::regclass) | false |  |  |  |
| entitlementno | varchar |  | true |  |  |  |
| employeeid | integer |  | true |  |  |  |
| salarystructureid | integer |  | true |  |  |  |
| startingdate | date |  | true |  |  |  |
| endingdate | date |  | true |  |  |  |
| applicabledate | date |  | true |  |  |  |
| inactivedate | date |  | true |  |  |  |
| isauthorized | boolean |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| seriescode | varchar |  | true |  |  |  |
| multientitlementid | integer |  | true |  |  |  |
| revision_no | integer |  | true |  |  |  |
| ctc | numeric |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pay_employee_entitlement_master_pkey | PRIMARY KEY | PRIMARY KEY (entitlementid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pay_employee_entitlement_master_pkey | CREATE UNIQUE INDEX pay_employee_entitlement_master_pkey ON public.pay_employee_entitlement_master USING btree (entitlementid) |

## Relations

![er](public.pay_employee_entitlement_master.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
