# public.sale_sipost_fielddetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| inv_post_fielddetailid | integer | nextval('sale_sipost_fielddetail_inv_post_fielddetailid_seq'::regclass) | false |  |  |  |
| invoiceid | integer |  | true |  |  |  |
| fieldid | integer |  | true |  |  |  |
| fieldvalue | text |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_sipost_fielddetail_pkey | PRIMARY KEY | PRIMARY KEY (inv_post_fielddetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_sipost_fielddetail_pkey | CREATE UNIQUE INDEX sale_sipost_fielddetail_pkey ON public.sale_sipost_fielddetail USING btree (inv_post_fielddetailid) |

## Relations

![er](public.sale_sipost_fielddetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)