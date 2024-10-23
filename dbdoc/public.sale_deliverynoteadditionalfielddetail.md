# public.sale_deliverynoteadditionalfielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| additionalfieldid | integer | nextval('sale_deliverynoteadditionalfielddetail_additionalfieldid_seq'::regclass) | false |  |  |  |
| transactionid | integer |  | false |  |  |  |
| itemdetailid | integer |  | false |  |  |  |
| fieldvalue | varchar |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_deliverynoteadditionalfielddetail_pkey | PRIMARY KEY | PRIMARY KEY (additionalfieldid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_deliverynoteadditionalfielddetail_pkey | CREATE UNIQUE INDEX sale_deliverynoteadditionalfielddetail_pkey ON public.sale_deliverynoteadditionalfielddetail USING btree (additionalfieldid) |

## Relations

![er](public.sale_deliverynoteadditionalfielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)