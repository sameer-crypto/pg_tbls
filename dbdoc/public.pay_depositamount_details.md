# public.pay_depositamount_details

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| advanceid | integer |  | true |  |  |  |
| depositid | integer |  | false |  |  |  |
| depositdetailid | integer | nextval('pay_depositamount_details_depositdetailid_seq'::regclass) | false |  |  |  |
| deposit | numeric(18,2) |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pay_depositamount_details_pkey | PRIMARY KEY | PRIMARY KEY (depositdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pay_depositamount_details_pkey | CREATE UNIQUE INDEX pay_depositamount_details_pkey ON public.pay_depositamount_details USING btree (depositdetailid) |

## Relations

![er](public.pay_depositamount_details.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
