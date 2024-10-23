# public.pay_deductionadjustmentmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| deductionid | integer | nextval('pay_deductionadjustmentmaster_deductionid_seq'::regclass) | false |  |  |  |
| monthid | integer |  | false |  |  |  |
| yearid | integer |  | true |  |  |  |
| isauthorized | boolean |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| payperiodid | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pay_deductiondetails_pkey | PRIMARY KEY | PRIMARY KEY (deductionid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pay_deductiondetails_pkey | CREATE UNIQUE INDEX pay_deductiondetails_pkey ON public.pay_deductionadjustmentmaster USING btree (deductionid) |

## Relations

![er](public.pay_deductionadjustmentmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)