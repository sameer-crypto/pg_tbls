# public.pur_challanfielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| challanfielddetailid | integer | nextval('pur_challanfielddetail_challanfielddetailid_seq'::regclass) | false |  |  |  |
| challanid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pur_challanfielddetail_pkey | PRIMARY KEY | PRIMARY KEY (challanfielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pur_challanfielddetail_pkey | CREATE UNIQUE INDEX pur_challanfielddetail_pkey ON public.pur_challanfielddetail USING btree (challanfielddetailid) |

## Relations

![er](public.pur_challanfielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
