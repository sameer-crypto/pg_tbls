# public.quotationitemfielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| quotationitemfielddetailid | integer | nextval('quotationitemfielddetail_quotationitemfielddetailid_seq'::regclass) | false |  |  |  |
| quotationdetailid | integer |  | true |  |  |  |
| quotationid | integer |  | true |  |  |  |
| itemid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| quotationitemfielddetail_pkey | PRIMARY KEY | PRIMARY KEY (quotationitemfielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| quotationitemfielddetail_pkey | CREATE UNIQUE INDEX quotationitemfielddetail_pkey ON public.quotationitemfielddetail USING btree (quotationitemfielddetailid) |

## Relations

![er](public.quotationitemfielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
