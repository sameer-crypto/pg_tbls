# public.prod_itemjobworktaxdetail_amendlog

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| taxdetailamendid | integer | nextval('prod_itemjobworktaxdetail_amendlog_taxdetailamendid_seq'::regclass) | false |  |  |  |
| taxdetailid | integer |  | true |  |  |  |
| jobworkid | integer |  | true |  |  |  |
| jobworkamendid | integer |  | true |  |  |  |
| taxid | integer |  | true |  |  |  |
| rate | numeric(5,2) |  | true |  |  |  |
| taxtemplateid | integer |  | true |  |  |  |
| taxtemplatedetailid | integer |  | true |  |  |  |
| taxformula | varchar(150) |  | true |  |  |  |
| taxformulavalue | varchar(150) |  | true |  |  |  |
| taxamount | numeric(12,2) | 0 | true |  |  |  |
| taxorder | integer |  | true |  |  |  |
| asperactual | boolean |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| prod_itemjobworktaxdetail_amendlog_pkey | PRIMARY KEY | PRIMARY KEY (taxdetailamendid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| prod_itemjobworktaxdetail_amendlog_pkey | CREATE UNIQUE INDEX prod_itemjobworktaxdetail_amendlog_pkey ON public.prod_itemjobworktaxdetail_amendlog USING btree (taxdetailamendid) |

## Relations

![er](public.prod_itemjobworktaxdetail_amendlog.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)